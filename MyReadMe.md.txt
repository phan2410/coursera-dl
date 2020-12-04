git clone https://github.com/phan2410/coursera-dl
cd coursera-dl
git checkout fix_bad_request_api_v3

# now go to chrome, using this extention https://links.jianshu.com/go?to=https%3A%2F%2Fchrome.google.com%2Fwebstore%2Fdetail%2Fcookiestxt%2Fnjabckikapfpffapmjgojcnbfjonfjfg%3Fhl%3Den
# to download cookies.txt
# login to coursera: https://www.coursera.org/learn/neural-networks-deep-learning
# get correspondent cookies.txt

cp <the path of cookies.txt>\cookies.txt  cookies.txt

Windows: .\coursera-dl.bat -c cookies.txt --video-resolution 720p --path <path> --subtitle-language en --download-quizzes --download-notebooks <your course name>
Linux: ./coursera-dl -c cookies.txt --video-resolution 720p --path /home/myuser/ --subtitle-language en --download-quizzes --download-notebooks <your course name>
# here <your course name> = neural-networks-deep-learning
# Add --specialization if it is the name of a specialization

## For more help, run $./coursera-dl --help

For one using docker,
$ docker-compose run coursera-dl
$ ./coursera-dl -c cookies.txt --video-resolution 720p --path /home/myuser/ --subtitle-language en --download-quizzes --download-notebooks <your course name>