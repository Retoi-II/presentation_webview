### Availability

- Django;
- AdminLTE Integrated;
- Initial Commit;

# Setup

### Install Django
`py -m pip install django`

### Development Setup
+ settings.py
```
DEBUG = True
```

+ import AdminLTE 3.2.0 dist folder into static/adminlte3.2.0@dist/

### Static Files Setup
```
import os
...

...
	TEMPLATES = [
    		{
        		...
        		'DIRS': [os.path.join(BASE_DIR, 'templates')],  # Tambahkan path ke folder templates
        		...
    		},
	]

...
	STATICFILES_DIRS = [
			os.path.join(BASE_DIR, 'static'),
	]

	STATIC_ROOT = os.path.join(BASE_DIR, 'staticfiles')
 ...

```
