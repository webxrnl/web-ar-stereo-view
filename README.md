# ar-stereo-view
This project is about trying to generate a stereoscopic view for web-based AR, similar to VR-mode.  This allows for an immersive web-AR experience with a headset like the Aryzon.


## Contribute

1. Fork this project

2. First navigate to directory you keep your projects and set following temporary environment variables

```
cd <your-projects>
GITHUB_USERNAME="<github-username>"
PROJECT_NAME="ar-stereo-view"
```
3. Clone the repo and setup the git remotes

```
git clone --origin github/"$GITHUB_USERNAME" git@github.com:${GITHUB_USERNAME}/ar-stereo-view.git $PROJECT_NAME
```

4. Add WebXR NL upstream

```
cd $PROJECT_NAME
git remote add github/webxrnl git@github.com:webxrnl/ar-stereo-view.git
```

5. Hack the and open pull request

make your edits

```
git add -A
git commit -m"your commit message"
git push
```

Which would make a commit under your fork, Now open `https://github.com:${GITHUB_USERNAME}/ar-stereo-view` in your browser and iopen pull request.

6. If you need to update your for just run

```
git fetch --all
git rebase github/webxrnl/master
git push
```
