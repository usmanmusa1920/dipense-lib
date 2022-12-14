An OSINT tool for IT ninjas


# How to use the library
First we recommend creating a virtual environment `python3 -m venv venv` and then activate it `source venv/bin/activate`

Once that finish now install the library using `pip install dipense` and wait for the installation basically the library was uploaded using `sdist` (Source Distribution)

After that create a new file let call it `route.py` in the file put the below code

```python
from dipense import payloads
from dipense.structure import helper



if __name__ == '__main__':
    payloads(helper)
```

save the file and navigate to where the file is located in terminal and your are ready to go

To find information about a domain name run the file like:

`python3 route.py payloadwho -d google.com` or 
`python3 route.py payloadwho --domain google.com`


To find information about an ip address run the file like:

`python3 route.py payloadip -i 198.3.11.7` or 
`python3 route.py payloadip --ip 198.3.11.7`

You can also specify a flag of `-o` or `--open` to `True` this will automatically open a webbrowser showing you where that ip address is located, like:

`python3 route.py payloadip -i 198.3.11.7 -o True` or 
`python3 route.py payloadip -i 198.3.11.7 --open True`


To find information about a phone number run the file like you see below, be sure to start with the country code of that phone number:

`python3 route.py payloadnum -n +2349083513047` or 
`python3 route.py payloadnum --number +2349083513047`


To see positional argument and flags available run the file without any flag or positional argument like:

`python3 route.py`


## Github and docker repository:

- https://github.com/usmanmusa1920/dipense-lib
- https://hub.docker.com/r/usmanmusa/dipense


Pull requests are welcome


There is a version of this library on docker hub repo @ `https://hub.docker.com/r/usmanmusa/dipense`
## DiPense at a glance (docker)

![DiPense at a glance](https://raw.githubusercontent.com/usmanmusa1920/dipense/master/screen-shot.png)
