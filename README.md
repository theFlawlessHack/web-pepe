# web-pepe

welcome to web-pepe 🐸<br>
with web-pepe you can understand the way firebase works in web apps.

### firebase setup
start off by going to https://console.firebase.google.com<br>
after logging into your gmail account, add a new project.

![alt text](https://github.com/theFlawlessHack/web-pepe/blob/gh-pages/images/gs_web.png "Getting Started Web and Firebase")


### html setup
In the head tag of your main .html file you want to incluse these firebase header scripts<br><br>
For the bare bone basics include
```
<script src="https://www.gstatic.com/firebasejs/4.2.0/firebase.js"></script>
<script src="https://www.gstatic.com/firebasejs/4.2.0/firebase-app.js"></script>
<script src="https://www.gstatic.com/firebasejs/4.2.0/firebase-database.js"></script>
```

To include user authentication and messaging include these two additional scripts in your head tags

```        
<script src="https://www.gstatic.com/firebasejs/4.2.0/firebase-auth.js"></script>
<script src="https://www.gstatic.com/firebasejs/4.2.0/firebase-messaging.js"></script>
```
For reference on how this should look please [click here](https://github.com/theFlawlessHack/web-pepe/blob/gh-pages/index.html#L2-L11).

<b>Initializing firebase in your html</b>
In script tags at the end within your body tags you can initialize Firbase.

```
  // Initialize Firebase
  var config = {
      apiKey: "YOUR_API_KEY",
      authDomain: "YOUR_PROJECT_ID.firebaseapp.com",
      databaseURL: "https://YOUR_PROJECT_ID.firebaseio.com",
      projectId: "YOUR_PROJECT_ID",
      storageBucket: "",
      messagingSenderId: "SenderId"
  };

  firebase.initializeApp(config);
```

### adding firebase in html

### writing data to your database
