# SnakeGames
Hello (ʘ‿ʘ)╯

Snake Games on your's terminal
<h3> Usage </h3>
<p> First compile file snakegames.cpp </p>

var copy = function(target) {
    var textArea = document.createElement('textarea')
    textArea.setAttribute('style','width:1px;border:0;opacity:0;')
    document.body.appendChild(textArea)
    textArea.value = target.innerHTML
    textArea.select()
    document.execCommand('copy')
    document.body.removeChild(textArea)
}

var pres = document.querySelectorAll(".comment-body > pre")
pres.forEach(function(pre){
  var button = document.createElement("button")
  button.className = "btn btn-sm"
  button.innerHTML = "copy"
  pre.parentNode.insertBefore(button, pre)
  button.addEventListener('click', function(e){
    e.preventDefault()
    copy(pre.childNodes[0])
  })
})


Key used :

- W for Up
- S for Down
- D for Right
- A for Left

You can play demo in here : https://replit.com/@FandhikaAzhar/snake#main.cpp
