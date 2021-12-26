# python-pit
DockerFiles used to create Python container sandboxes specific to a use case. 

# use
build image, including `requirements.txt`\
`docker build --pull --rm -f "DockerFile-[use case]" -t python-pit:[use case] "."`

launch image, enter interactive cli (bash)\
`docker container run -it --name [use case] --entrypoint bash python-pit:[use case]`

kill and destroy container\
`docker kill [use case] && docker container prune -f`

