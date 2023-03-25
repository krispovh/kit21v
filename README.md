# kit21v
PS3="Select the programm: "

select opt in programm apache2 mysql php; do

	case $opt in
	apache2)
	sudo apt install apache2
	;;
	mysql)
	sudo apt install mysql-server
	;;
	php)
	sudo apt install php libapache2-mod-php php-mysql
	;;
	quit)
	break
	;;
	*)
	echo "Invalid programm $REPLY"
	;;
	esac
done
