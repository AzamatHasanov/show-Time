# show-Time
<script> // Function to display the time function showTime() { const date = new Date(); // Create a new Date object to get the current date and time let hours = date.getHours(); // Get the current hours let minutes = date.getMinutes(); // Get the current minutes let seconds = date.getSeconds(); // Get the current seconds // Format the time (add leading zero if the value is less than 10) hours = hours < 10 ? '0' + hours : hours; // If hours < 10, add a leading zero minutes = minutes < 10 ? '0' + minutes : minutes; // If minutes < 10, add a leading zero seconds = seconds < 10 ? '0' + seconds : seconds; // If seconds < 10, add a leading zero // Display the time on the page document.getElementById('clock').innerHTML = hours + ':' + minutes + ':' + seconds; // Call the showTime function again after 1 second (1000 ms) to update the time setTimeout(showTime, 1000); } // Start the function showTime(); </script>