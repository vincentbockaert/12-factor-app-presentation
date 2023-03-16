# 2 - Dependencies 

## Explicity declare and isolate dependencies

*Some example code below...*

1. Create a new virtual environment

```bash
python3 -m venv myapp-env
```

2. Activate the virtual environment

```bash
source myapp-env/bin/activate
```

3. Install the required packages with pip (python's package manager)

```bash
pip install -r requirements.txt
```

4. The `requirements.txt` file should contain a list of all the required packages and their versions. For example:

```makefile
flask==2.1.0
requests==2.26.0
``` 

This declares that the app requires Flask version 2.1.0 and Requests version 2.26.0. By declaring dependencies explicitly in this way, we can ensure that the app will run with the correct versions of its dependencies, regardless of what other packages may be installed system-wide.

5. Run the app:

```bash
python app.py
```

This runs the app within the virtual environment, which ensures that no implicit dependencies "leak in" from the surrounding system.

Note that this is just one example, and other programming languages and tools may have different ways of declaring and isolating dependencies. However, the principles of explicit declaration and isolation apply universally to twelve-factor apps.