Naruto Quotes Api
====================
Simple app to generate random Naruto quotes using Python and Flask

# Running locally
With Python and Pip installed, install the dependencies with:
```sh
pip install -r requirements.txt
```

Run with the Flask dev server (quick testing):
```sh
python3 app.py
```

Or run with Gunicorn (recommended):
```sh
gunicorn --config gunicorn.conf.py app:NarutoApi
```

# Running with Docker
Build the image:
```sh
docker build -t naruto-quotes-server .
```

Run the container:
```sh
docker run -p 5000:5000 naruto-quotes-server
```

The API will be available at `http://localhost:5000/`.

# License
This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details
