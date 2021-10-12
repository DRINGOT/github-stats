# Installation

<!-- TODO: Add details and screenshots -->

1. Create a personal access token (not the default GitHub Actions token) using
   the instructions
   [here](https://docs.github.com/en/github/authenticating-to-github/creating-a-personal-access-token).
   Personal access token must have permissions: `read:user` and `repo`. Copy
   the access token when it is generated – if you lose it, you will have to
   regenerate the token.
2. Fork the repository.
3. Go to the "Settings" tab of the fork and go to the "Secrets" page (bottom
   left). Create a new secret with the name `ACCESS_TOKEN` and paste the copied
   personal access token as the value.
4. Go to the "Actions" tab of the fork and hit the big green button to enable
   Actions.
5. If you want to ignore certain repos, add them (separated by commas) to a new
   secret—created as before—called `EXCLUDED`.
6. Commit a small change to the repo (for example remove a newline from the end
   of the README) to force it to regenerate the stats images. The first time
   that it generates the stats images, it may take a ~very~ long time. It does 
   not generally take as long as the first time when it runs in the future.
7. Check out the images that have been created in the `generated` folder.
8. Link back to this repository so that others can generate their own 
   statistics images.
9. Star this repo if you like it!
