## IFRAME's are fun
I frames are fun. plug and play from the outside. 

no external javascript allowed inside the iframe black box.

but still many creative things are possible.

Also flashing Iframes can bring your computer to its full potential

Soo many network requests 😍<br/>
The possibilities are endless!

## Original Idea
A while back I was learning tachyons css and struggling with their components section.
```
http://tachyons.io/components/
http://tachyons.io/components/article-lists/title-preview-author-media-flipped/index.html
http://tachyons.io/components/article-lists/title-preview-author-media/index.html
http://tachyons.io/components/articles/feature/index.html
http://tachyons.io/components/articles/full-bleed-background/index.html
http://tachyons.io/components/articles/headline-title-text/index.html
```

I asked myself:<br/>
Wouldn't it be nice if my browser could quickly cycle through the entire component route directory allowing me to find inspiration, pause and capture the styles for my website.

## Project Objectives
1) "flash iframes", "loading background Iframe so there is no lag in transition from 1 iframe to the next"
2) "pause" button, stops "iframe flash" so that styles can be inspected and applied to another application.
3) "go back" an iframe, allows users to cycle backwards without flashing (slight delay), also pauses "iframe flashing"
4) hitting "play" will resume will "iframe flashing" from "go back" or "pause" state


## This Project
```javascript
function buildIframes( index ) {
  /* 
  Step 1) immediately load iframe no. index + 1
  Step 2) immediately load iframe no. index + 2 with display none
  Step 3) wait 3 seconds
  Step 4) remove no. 2 display none style
  Step 5) remove iframe no 1 from dom.
  */
}

function sleepAndRun(index) {
  setTimeout(() => {
    buildIframes(index);
    sleepAndRun++
  }, 2000);
}
```

## Future
Ultimately this could become a chrome plugin to grab urls and start "iframe flashing" when user clicks plugin.
