// Step 1: Define displayMessage function
function displayMessage(name) {
  console.log(`Hello, ${name}!`);
}

// Step 2: Define getUserInput function with a callback
function getUserInput(callback) {
  setTimeout(() => {
    const username = "Alice"; // Simulated fetched username
    callback(username);       // Calling the callback
  }, 1000);
}

// Calling the function
getUserInput(displayMessage);
