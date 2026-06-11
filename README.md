# downsub-bookmarklet
a simple javascript bookmarklet to submit the current URL to downsub (subtitle.to) in a new window/tab for use with youtube videos

i made this because i frequently download subtitles/captions from youtube videos, and i'm sick of copy/pasting the URL+changes into a new tab.

---

base javascript:
`var baseUrl = "https://subtitle.to/"
var urlmod = document.URL
window.open(baseUrl + urlmod, '_blank')`

html: 
`<a href="javascript:(function()%7Bvar%20baseUrl%20%3D%20%22https%3A%2F%2Fsubtitle.to%2F%22%0Avar%20urlmod%20%3D%20document.URL%0Awindow.open(baseUrl%20%2B%20urlmod%2C%20'_blank')%7D)()%3B">💬 downsub this 💬</a>`

markdown:
`[💬 downsub this 💬](javascript:\(function\(\)%7Bvar%20baseUrl%20%3D%20%22https%3A%2F%2Fsubtitle.to%2F%22%0Avar%20urlmod%20%3D%20document.URL%0Awindow.open\(baseUrl%20%2B%20urlmod%2C%20'_blank'\)%7D\)\(\)%3B)`

markdown (live link)  
[💬 downsub this 💬](javascript:\(function\(\)%7Bvar%20baseUrl%20%3D%20%22https%3A%2F%2Fsubtitle.to%2F%22%0Avar%20urlmod%20%3D%20document.URL%0Awindow.open\(baseUrl%20%2B%20urlmod%2C%20'_blank'\)%7D\)\(\)%3B)

---

made with help from [caiorss @ github](https://github.com/caiorss/bookmarklet-maker) and [mrcoles.com](https://mrcoles.com/bookmarklet/) generators to double-check my code
