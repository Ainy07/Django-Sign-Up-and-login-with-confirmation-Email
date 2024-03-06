# Django-Sign-Up-and-login-with-confirmation-Email
using django



To create a virtual environment for your Django project, you can use virtualenv or venv (if you are using Python 3.3 or newer). Here's how you can do it using venv:

Open a terminal or command prompt.

Navigate to your project directory.

Run the following command to create a virtual environment named env (you can replace env with any name you prefer):

bash
Copy code
python -m venv env
Activate the virtual environment. On Windows, run:

bash
Copy code
env\Scripts\activate
On macOS and Linux, run:

bash
Copy code
source env/bin/activate
Your virtual environment is now activated. You should see (env) in your command prompt.

To install django-crispy-forms in your Django project, you can use pip. First, make sure your virtual environment is activated. Then, run the following command:

bash
Copy code
pip install django-crispy-forms
Once the installation is complete, add 'crispy_forms' to the INSTALLED_APPS in your Django settings file (settings.py):

python
Copy code
INSTALLED_APPS = [
    ...
    'crispy_forms',
    ...
]
Next, add the following line to specify the template pack you want to use (e.g., bootstrap4, bootstrap3, uni-form, etc.). Add this line after the INSTALLED_APPS in your settings file:

python
Copy code
CRISPY_TEMPLATE_PACK = 'bootstrap4'
Finally, to use crispy forms in your templates, load the crispy forms template tag at the top of your template file:

html
Copy code
{% load crispy_forms_tags %}
You can then use crispy forms in your Django templates to render your forms with the specified template pack.



##please use your Email and Password


clone the repo --
git clone https://github.com/Ainy07/Django-Sign-Up-and-login-with-confirmation-Email


##setting.py

EMAIL_BACKEND = 'django.core.mail.backends.smtp.EmailBackend'
EMAIL_HOST = 'smtp.gmail.com'
EMAIL_PORT = 587
EMAIL_USE_TLS = True
EMAIL_HOST_USER = 'your_email@gmail.com'
EMAIL_HOST_PASSWORD = 'your_email_password'

