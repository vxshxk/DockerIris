1. Dockerized the rails application by adding the Dockerfile(its content being from the officiaal docker image of rails) and entrypoint.sh file.
2. But I got this error![Screenshot (20)](https://user-images.githubusercontent.com/115456558/230730378-48b02726-97ed-4bcd-a06f-eadb3b41ce0d.png)
But then looked up ffor the error on stackoverflow, got to know all I had to do was to delete the gemlock file and re run thee docker build command.
3. Once I did that, I got another error![Screenshot (22)](https://user-images.githubusercontent.com/115456558/230730473-7981e496-0614-401a-8fa5-1f13fcc97b59.png)
4. Then I just changed the command FROM ruby 2.5 in the dockerfile to FROMruby 3.1.3, it worked.
