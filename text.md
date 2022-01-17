wallpaper API = https://apis.scrimba.com/unsplash/photos/random?orientation=landscape&query=nature




fetch("https://apis.scrimba.com/unsplash/photos/random?orientation=landscape&query=dog")
    .then(res => res.json())
    .then(data => {
        document.body.style.backgroundImage = `url(${data.urls.regular})`
		document.getElementById("author").textContent = `By: ${data.user.name}`
    })
    .catch(err => {
        // Use a default background image/author
        document.body.style.backgroundImage = `url(https://images.unsplash.com/photo-1560008511-11c63416e52d?crop=entropy&cs=tinysrgb&fit=max&fm=jpg&ixid=MnwyMTEwMjl8MHwxfHJhbmRvbXx8fHx8fHx8fDE2MjI4NDIxMTc&ixlib=rb-1.2.1&q=80&w=1080
)`
		document.getElementById("author").textContent = `By: Dodi Achmad`
    })

data.weather[0].main


background: rgba(0, 0, 0, 0.479);
    backdrop-filter: saturate(180%) blur(10px);



some inovation:-
1) Live Weather Wall Paper✅
2) Remove DogeCoin API
3) Add Some Styling In Display Content's (like: Time, Author, Weather)