#!/usr/bin/env bash
# Create a .pid file on /var/run and this process can be killed (Have special interactions)
trap "echo \"Y U no love me?!\"; exit" SIGINT
trap "sudo rm /var/run/myscript.pid; exit" SIGQUIT
trap "echo \"I hate the kill command\"; sudo rm /var/run/myscript.pid; exit" SIGTERM

echo "$$" > /var/run/myscript.pid

while true
do
	echo "To infinity and beyond"
	sleep 2
done
