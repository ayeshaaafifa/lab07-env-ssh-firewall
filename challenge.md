# Lab 7 Challenge: Environment Audit and Ping Block



## Task 1: PATH, LANG and PWD



Command: printenv | grep PATH

Answer: PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/games:/usr/local/games:/snap/bin



Command: printenv | grep LANG

Answer: LANG=en_GB.UTF-8



Command: printenv | grep PWD

Answer: PWD=/home/ayeshaaafifa/lab07-env-ssh-firewall



## Task 2: Student variables with export



Commands:

export STUDENT_NAME="Ayesha"

export STUDENT_ROLL_NUMBER="FA24B1-SE-001"

export STUDENT_SEMESTER="5"



Show all three with one command: printenv | grep '^STUDENT_'

Answer:

STUDENT_NAME=Ayesha

STUDENT_SEMESTER=5

STUDENT_ROLL_NUMBER=FA24B1-SE-001



Proof they are gone: I ran exit, logged in again and ran

printenv | grep '^STUDENT_'

Answer: it showed nothing, because export only lasts for the current session.



## Task 3: Make the variables permanent



Commands: added these lines to the end of ~/.bashrc using vim ~/.bashrc

export STUDENT_NAME="Ayesha"

export STUDENT_ROLL_N
