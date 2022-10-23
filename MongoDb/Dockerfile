#step1:Getting base image (an operating system)
FROM alpine


#step2:Install a software

# https://dl-cdn.alpinelinux.org/alpine/v3.16/main/x86_64/APKINDEX.tar.gz

RUN echo 'https://dl-cdn.alpinelinux.org/alpine/v3.6/main' >> /etc/apk/repositories
RUN echo 'https://dl-cdn.alpinelinux.org/alpine/v3.6/community' >> /etc/apk/repositories
RUN apk update
RUN apk add mongodb=3.4.4-r0
# in the above command we are installing software binutils

#step2.1:configure the software
VOLUME [ "/data/db" ] 
WORKDIR /data
EXPOSE 27017

# you can write your codes here

#step3:set default commmands

CMD ["mongod"]
#you can write the default commads here as COMMAND ["npm","install"]

#Adding a comment for Testing purpose
