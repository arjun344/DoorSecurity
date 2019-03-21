<button id="0" onclick="myfunc()">open</button>
<button id="1" onclick="myfunc()">close</button>


<script src="https://www.gstatic.com/firebasejs/5.9.0/firebase.js"></script>
<script src="https://www.gstatic.com/firebasejs/5.9.0/firebase-app.js"></script>

<!-- Add additional services that you want to use -->
<script src="https://www.gstatic.com/firebasejs/5.9.0/firebase-auth.js"></script>
<script src="https://www.gstatic.com/firebasejs/5.9.0/firebase-database.js"></script>
<script src="https://www.gstatic.com/firebasejs/5.9.0/firebase-firestore.js"></script>
<script src="https://www.gstatic.com/firebasejs/5.9.0/firebase-messaging.js"></script>
<script src="https://www.gstatic.com/firebasejs/5.9.0/firebase-functions.js"></script>
<script>
  // Initialize Firebase
  // TODO: Replace with your project's customized code snippet
  var config = {
    apiKey: "AIzaSyDUDJRUAhcnG1lP9saN_B7GaygCXCC3264",
    authDomain: "securitydoor-a1d79.firebaseapp.com",
    databaseURL: "https://securitydoor-a1d79.firebaseio.com",
    projectId: "securitydoor-a1d79",
  };
  firebase.initializeApp(config);
  var database = firebase.database().ref();
  function myfunc()
  {
    database.set({
      status:parseInt(document.activeElement.id)
    });
  }
</script>
