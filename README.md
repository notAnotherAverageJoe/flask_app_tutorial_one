Welcome back to Byte Brewmaster! In our first tutorial, we’re diving into web development by building a simple web app using Flask and JavaScript. Whether you're new to web development or looking to brush up on your skills, this guide will walk you through setting up Flask, creating routes, and adding interactivity with JavaScript. Let's get started!


## Prerequisites

Before we begin, make sure you have the following:
- Basic understanding of Python and JavaScript
- Python installed on your machine
- Flask installed (`pip install Flask`)
- A code editor (such as VS Code)


## Step 1: Setting Up Your Flask Environment

First, we need to set up our development environment. Open your terminal and follow these steps:

1. Create a new directory for your project:
    ```bash
    mkdir my_flask_app
    cd my_flask_app
    ```

2. Set up a virtual environment:
    ```bash
    python -m venv venv #may need to type python3 -m venv venv
    source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
    ```

3. Install Flask:
    ```bash
    pip install Flask
    ```

4. Create a new file called `app.py` and open it in your code editor.

## Step 2: Creating Your Flask App

Let's create a basic Flask application. In `app.py`, add the following code:

```python
from flask import Flask, render_template

app = Flask(__name__)

@app.route('/')
def home():
    return render_template('index.html')

if __name__ == '__main__':
    app.run(debug=True)



## Step 3: Adding Templates

Next, we'll add an HTML template. Create a new directory called `templates` in your project folder, and inside it, create a file named `index.html`. Add the following content:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>make up a name!</title>
</head>
<body>
    <h1>Welcome to My name it!</h1>
    <button id="myButton">Click Me!</button>
    <script src="{{ url_for('static', filename='script.js') }}"></script>
</body>
</html>

## Step 4: Adding Static Files

Create a directory named `static` in your project folder, and inside it, create a file named `script.js`. Add the following JavaScript code:

```javascript
document.getElementById('myButton').addEventListener('click', function() {
    alert('Button clicked!');
});
# this will pop up an alert on your screen letting you know that the button has been clicked!


## Step 5: Running Your App

With everything set up, it's time to run your Flask app. In your terminal, make sure you're in your project directory and your virtual environment is activated, then run:

```bash
python app.py

"If you enjoyed this tutorial, don't forget to subscribe to Byte Brewmaster for more coding adventures. Share this post with fellow developers, and let me know in the comments what you'd like to learn next. Let's continue brewing some awesome code together!"

YOU DID IT!
"Congratulations! You've just built a simple web app using Flask and JavaScript. We've covered setting up your environment, creating a Flask app, adding templates, and using JavaScript for interactivity. This is just the beginning. In future posts, we'll dive deeper into building more complex features, handling forms, and connecting to databases"

"This is a simple example of developing a website or web app from scratch, and the progress that you made today whether you are new to programming or have been doing it a while, practiciing the fundementals create a solid foundation to build a life and career upon."