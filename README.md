# Django Volumes
Django Volume Template for Railway

This template is a great starter if you are looking to use Railway Volumes with your Django project for user uploaded media files. It takes all the complexity out of configuring your project for serving files.

No more help channel because you can't get volumes to work!

## Troubleshooting
If you get the following error `No such file or directory: '/app/media/directory/...'` make sure your directory exists since your folder structure has to be build from scratch for production purpose on the persistent storage.

You can use something like this:

```python
new_directory = os.path.join(settings.MEDIA_ROOT, 'directory')
if not os.path.exists(new_directory):
  os.makedirs(new_directory)
```

## Deploy
[![Deploy on Railway](https://railway.app/button.svg)](https://railway.app/template/AWUIv6)
