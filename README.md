from flask import Flask

app = Flask(__name__)

@app.route('/')
def home():
    return "<h1>Welcome to My Website</h1><p>This is a simple homepage.</p>"

@app.route('/about')
def about():
    return "<h1>About Page</h1><p>This page tells you about this site.</p>"

if __name__ == '__main__':
    app.run(debug=True)
