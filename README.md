# Wifi-Deauth-Attack
    Commmand Line Tool

    This Python script performs a WiFi deauthentication attack on a selected wireless network. The script first checks for any existing .csv files in the current
    working directory, moves them to a /backup directory, and creates a new .csv file to store the results of the attack. It then prompts the user to select a
    wireless interface to use for the attack, and puts it into monitored mode using the airmon-ng utility.

    The script uses the airodump-ng utility to discover access points and continuously updates the results in the .csv file. It then displays the list of access
    points and prompts the user to select a target by ESSID. Once the target is selected, the script uses the aireplay-ng utility to launch a deauthentication
    attack against the target.

    The script also includes error handling, such as checking for the presence of a WiFi adapter and ensuring that the user enters a valid input when selecting a
    wireless interface or target ESSID.


    #USAGE

        Connect your wireless interface
        Run the script with sudo privileges: sudo python3 wifi_dos.py
        Select the WiFi interface you want to use for the attack
        Wait for available networks to be displayed, and select the one you want to attack
        Press Ctrl+C to begin the attack
        To quit any inifinite loop , press Ctrl + c.


    NOTES

        This script is for educational purposes only. The author does not condone illegal or unethical use of this script.
        The script may not work on all WiFi adapters and drivers.
        If the script fails to find any wireless networks, try moving closer to a wireless access point.

    Requirements

        A WiFi adapter that supports monitor mode
        Aircrack-ng (install with sudo apt install aircrack-ng)


    

    Note: Please use this script only for educational purposes and do not use it for any illegal or malicious activities. The author is not responsible for any damage caused by its usage.

