import chromelogger as console
from django.http import HttpResponse


def index(request):
    response = HttpResponse("Hello, world. You're at the poll index.")
    console.log('Hello console!')
    console.log(request.user)
    return response
