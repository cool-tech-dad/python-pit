# python-pit
DockerFiles used to create Python container sandboxes specific to a use case. 

# use
build image, including `requirements.txt`\
`docker build --pull --rm -f "DockerFile-fooBar" -t python-pit:fooBar"."`

launch image, enter interactive cli (bash)\
`docker container run -it --name fooBar --entrypoint bash python-pit:fooBar`

kill and destroy container\
`docker kill fooBar && docker container prune -f`

fooBar = use case identifier

