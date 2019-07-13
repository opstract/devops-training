# User Management tasks:
1. Create the users **Serena Williams**, **Venus Williams** and **Justine Henin**, all of them with password set to **stargate**, with username **(lower case!)** as their first name, and their full name in the comment. Verify that the users and their home directory are properly created.
2. Create a user called **kornuser**, give him the Korn shell **(/bin/ksh)** as his default shell. Login with this user.
3. Create a user named **einstime** without a home directory, give him **_/bin/date_** as his default login shell. What happens when you login with this user ? Can you think of a useful real world example for changing a user's login shell to an application ?
4. Try the commands **who, whoami, who am i, w, id, echo $USER $UID** . 
5. 
- Lock the **venus** user account with **usermod**.
- Use **passwd -d** to disable the **serena** user's password. Verify the serena line in **_/etc/shadow_** before and after disabling.
- What is the difference between locking a user account and disabling a user account's password ?
6. As **root** change the password of **einstime** to **stargate**.
7. Now try changing the password of **serena** to **"serena as serena"**.
8. Make sure every new user needs to change his password every **10** days.
9. Set the **warning** number of days to **four** for the **kornuser**.

10. 
- Set the password of two separate users to **stargate**. Look at the encrypted stargate's in **_/etc/shadow_** and explain why they are different? Also how we can unified the encrypted stargate password inside the **_/etc/shadow_** without editing the file ?
- Take a backup as root of **_/etc/shadow_**. Use vi/vim to copy an encrypted **stargate** to another user. Can this other user now login with **stargate** as a password ?
11. Put a file in the **skeleton directory (/etc/skel/)** and check whether it is copied to user's home directory. When is the skeleton directory copied ?
12. Why we use **vipw** instead of **vi/vim** ? What could be the problem when using vi or vim ? 
13. List all the shells inside **_/etc/shells_** then change your login shell to the **system shell**, log out and back in. Now change back to **bash shell**. 
14. Which **useradd** option allows you to name a home directory ?
15. How can you see whether the password of user **harry** for example is locked or unlocked ? Give a solution with **grep** and a solution with **passwd**.
