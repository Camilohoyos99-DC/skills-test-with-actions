<header>
<!-- trigger ci.yml -->

<!--
  <<< Author notes: Course header >>>
  Include a 1280×640 image, course title in sentence case, and a concise description in emphasis.
  In your repository settings: enable template repository, add your 1280×640 social image, auto delete head branches.
  Add your open source license, GitHub uses MIT license.
-->

# Test with Actions

_Create workflows that enable you to use Continuous Integration (CI) for your projects._

</header>

<!--
  <<< Author notes: Step 2 >>>
  Start this step by acknowledging the previous step.
  Define terms and link to docs.github.com.
-->

## Step 2: Fix the test

_Great job adding the templated workflow! :tada:_

Adding that file to this branch is enough for GitHub Actions to begin running CI on your repository.

When a GitHub Actions workflow is running, you should see some checks in progress, like the screenshot below.

<img alt="checks in progress in a merge box" src=https://user-images.githubusercontent.com/16547949/66080348-ecc5f580-e533-11e9-909e-c213b08790eb.png width=400 />

You can follow along as GitHub Actions runs your job by going to the **Actions** tab or by clicking "Details" in the merge box below.

When the tests finish, you'll see a red X :x: or a green check mark :heavy_check_mark: in the merge box. At that point, you can access the logs for the build job and its associated steps.

_By looking at the logs, can you identify which tests failed?_ To find it, go to one of the failed builds and scroll through the log. Look for a section that lists all the unit tests. We're looking for the name of the test with an "x".

<img alt="screenshot of a sample build log with the names of the tests blurred out" src=https://user-images.githubusercontent.com/16547949/65922013-e740a200-e3b1-11e9-8151-faf52c30201e.png width=400 />

If the checks don't appear or if the checks are stuck in progress, there's a few things you can do to try and trigger them:

- Refresh the page, it's possible the workflow ran and the page just hasn't been updated with that change.
- Try making a commit on this branch. Our workflow is triggered with a `push` event, and committing to this branch will result in a new `push`.
- Edit the workflow file on GitHub and ensure there are no red lines indicating a syntax problem.

### :keyboard: Activity: Fix the test

1. Update the contents in the `ci` branch to get the test to pass. You need to look at the logs to see what caused the test to fail.
1. **Commit changes**.
1. Wait about 20 seconds and then refresh this page (the one you're following instructions from). [GitHub Actions](https://docs.github.com/actions) will automatically update to the next step.

<footer>

<!--
  <<< Author notes: Footer >>>
  Add a link to get support, GitHub status page, code of conduct, license link.
-->

---

Get help: [Post in our discussion board](https://github.com/orgs/skills/discussions/categories/test-with-actions) &bull; [Review the GitHub status page](https://www.githubstatus.com/)

&copy; 2023 GitHub &bull; [Code of Conduct](https://www.contributor-covenant.org/version/2/1/code_of_conduct/code_of_conduct.md) &bull; [MIT License](https://gh.io/mit)

</footer>
