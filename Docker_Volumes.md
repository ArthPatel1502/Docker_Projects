ubuntu@ip-172-31-16-27:~/docker$ docker volume create arth
>> arth

ubuntu@ip-172-31-16-27:~/docker$ docker volume inspect arth
>>
[
    {
        "CreatedAt": "2026-07-10T03:49:25Z",
        "Driver": "local",
        "Labels": null,
        "Mountpoint": "/var/lib/docker/volumes/arth/_data",
        "Name": "arth",
        "Options": null,
        "Scope": "local"
    }
]

ubuntu@ip-172-31-16-27:~/docker$ docker run -d --mount source=arth,target=/app ubuntu:latest
>> 5a5043c266de3a90b9274c7231ccd0cee4170c0e3573242175137ff0538c3264
