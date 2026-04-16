# a2retrotech
Landing page for A2 Retro Tech sign up

The test site URL is https://test.a2retrotech.com/

## Making edits

All edits made to this site will be deployed within a few minutes to https://test.a2retrotech.com/ - this is the easiest way to test the site.

## Testing locally

You can also make edits locally and not wait for deployment. This would require both `git` and `python` being installed which are both cross platform tools and should be available for any OS. This can also be done with GitHub Desktop, though I'm not familiar with that program.

1. Clone the repo: `git clone git@github.com:artlogic/a2retrotech.git` (you'll need to setup a SSH key with github to do this: https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent)
2. Make changes to the files on your system.
3. Test the site by running: `python -m http.server` - this start a local server at the address/port displayed by Python. You can then view the site in your browser.
4. Once you are happy, add, commit, and push your changes, for example:
    1. `git add index.html`
    2. `git commit -m 'Updated page for April`
    3. `git push`
5. If everything went well, the test site should be updated shortly with your changes.

## Deploying changes to production

Once you are happy with the test site, you can move changes to production. This assumes you are working with a local clone of the repo. There's currently no way to do this from the website, though I imagine GitHub Desktop might have a way.

1. Verify you are on the `main` branch: `git status` (look for `On branch main`).
2. Update `main` with any changes from the remote repo: `git pull`.
3. Move to the `publish` branch: `git checkout publish`.
4. Merge changes from `main`: `git merge main` (this may prompt you for a merge message or bring up an editor - you can just use the default here).
5. Publish the changes: `git push`.
6. Switch back to `main`: `git checkout main`.

The production site should be updated within the next 3-4 minutes.
