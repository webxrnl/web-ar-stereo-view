# web-ar-stereo-view
This project is about trying to generate a stereoscopic view for web-based AR, similar to VR-mode.  This allows for an immersive web-AR experience with a headset like the Aryzon or other cardboard.

## Stereo camera-feed
There are of course different ways to go about this, but I thought it would be nice to try a 'simple and elegant' solution first:
splitting the world up in stereo, before it enters the camera-lens.  This can easily be achieved with some mirrors, like in this universal 3D camera lens:

![Universal 3D camera lens](https://www.promostore.nl/media/catalog/product/cache/3/image/9df78eab33525d08d6e5fb8d27136e95/p/3/d305df47b42a46d8bb069de8d59caf49/Relatiegeschenk-Universele-3D-camera-lens-882425562.jpg)

![3D camera lens in use](https://www.promostore.nl/media/catalog/product/cache/3/image/9df78eab33525d08d6e5fb8d27136e95/p/3/c690dd6970f7e0abbbcecb1f4314284c/Relatiegeschenk-Universele-3D-camera-lens-882425562.jpg)

These are actually designed to record something in stereo that can later be played back in a VR headset.
I've tried this setup and it works!  In the Aryzon cardboard headset, the 'real' window to the world needs to be covered though, to see only the stereoscopic camera view.  In the normal cardboard, you need to make some modifications to allow for some room for the camera and clip-on.


## Stereo rendering of augmented layer
This, I feel, we are doing already with web-VR in VR-mode. I would like to see if it is possible to use this with a transparent background.


## Contribute

1. Fork this project

2. First navigate to directory you keep your projects and set following temporary environment variables

```
cd <your-projects>
GITHUB_USERNAME="<github-username>"
PROJECT_NAME="web-ar-stereo-view"
```
3. Clone the repo and setup the git remotes

```
git clone --origin github/"$GITHUB_USERNAME" git@github.com:${GITHUB_USERNAME}/web-ar-stereo-view.git $PROJECT_NAME
```

4. Add WebXR NL upstream

```
cd $PROJECT_NAME
git remote add github/webxrnl git@github.com:webxrnl/web-ar-stereo-view.git
```

5. Hack the and open pull request

make your edits

```
git add -A
git commit -m "your commit message"
git push
```

Which would make a commit under your fork, Now open `https://github.com:${GITHUB_USERNAME}/web-ar-stereo-view` in your browser and open pull request.

6. If you need to update your fork just run

```
git fetch --all
git rebase github/webxrnl/master
git push
```
