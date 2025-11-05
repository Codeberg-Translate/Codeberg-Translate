## Codeberg Translate GitHub Bot
Codeberg Translate uses Weblate. Have a look at [Weblate's documentation](https://docs.weblate.org/) if you have any questions.

To use Codeberg Translate for pushing to GitHub:
- Navigate to your Codeberg Translate Project.
- Navigate to whatever Component you want to push to GitHub.
- Enter the Component's settings.
- Got to the "Version control" tab.
- Set the relevant GitHub repository in the `Repository push URL` field. E.g. `git@github.com:USERorORGANIZATION/REPOSITORY.git`
Codeberg Translate will use @codeberg-translate for pushing to GitHub. Weblate currently doesn't allow commiting/pushing as a different user.
- Invite `@Codeberg-Translate` as a collaborator to your GitHub repository. This account accepts collaboration requests within 10 minutes.
After the invite was automatically accepted, Codeberg Translate should now be able to push to your repository.
- Add `https://translate.codeberg.org/hooks/github/` as a Webhook to your GitHub repository (leaving "Content-Type" as is). This notifies Codeberg Translate of any changes to your repository, so it can pull them immediately.

For more information please refer to: https://docs.weblate.org/en/latest/admin/continuous.html
