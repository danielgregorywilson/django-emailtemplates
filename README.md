![Concentric Sky](https://concentricsky.com/media/uploads/images/csky_logo.jpg)


# Django Email Templates

Email Templates is a Django app to allow creation and editing of email templates in the admin. The resulting templates can be referenced in code and will be rendered with standard Django template context.


## Installation

    pip install git+https://github.com/concentricsky/django-emailtemplates.git

Include Email Templates in your settings.py.

    INSTALLED_APPS = [

    	...

    	'emailtemplates',

        ...
    ]

Send an email by using the send_email_template utility.

	from emailtemplates.utils import send_email_template
    send_email_template('template_slug', 'toemail@example.com', {'context_variable': 'foo'})

