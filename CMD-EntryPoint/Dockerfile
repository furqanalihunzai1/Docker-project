FROM alpine

#ENTRYPOINT ["/bin/echo", "Hello world"]

#CMD ["/bin/echo" , "Hello world"]

ENTRYPOINT ["/bin/echo"]
CMD [ "Hello world" ]

#So, whenever we use CMD in our docker file it will
#docker command that has been set after the executable(/bin/echo)
#and when we pass the command through CLI It will override
#the default parameter in CMD and run the new parameter.
#While in ENTRYPOINT the executeable is set as default
#container startup and whenever we pass a parameter through CLI It
#won't override it will append that parameter it is end and run that parameter too.

