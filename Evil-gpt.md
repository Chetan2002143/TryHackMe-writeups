# Evil-GPT Walkthrough

In this room, I'll walk you through how I got this AI chatbot to spill out the flag!  
It’s an easy room which requires basic Linux knowledge and a bit of Prompt Engineering.

---

## Steps Taken
1. Ran `pwd` → confirmed shell commands worked.
2. Ran `ls` → found `evilai.py`.
3. Used `locate` and `find` to search for the flag.
4. Checked `/root` → found `flag.txt`.
5. Tried `cat /root/flag.txt` (failed).
6. Used `strings /root/flag.txt` → **Flag Found! 

---

## Key Takeaways
- Misconfigured chatbot allowed shell commands.
- Prompt engineering + Linux basics = success.

The task might seem a bit confusing, but all we really need to do is interact with the chatbot and take advantage of its misconfigured setup to extract the flag.

After connect to the machine,

You can’t interact with ai like others like asking anything, if you do, it’ll stuck. You have to command this as a terminal.

First, I gave it the command “pwd” to get to know the working directory but it didn’t give me anything relevant. But it confirmed that shell command was being executed.
 
Now, I ran “ls” to list files in the current directory, I find evilai.py script, tried to run the file, but it says “Address already in use”. 
Yes, this means exactly what you’re thinking. This was our chatbot.
 
Now, we are tasked to find the flag. So, I use the “locate” and “find” command.

I tried some more commands to find the path of the flag. Then, I use “ls  /root” command and there was the flag. (flag.txt)

Now, I have to print the flag. So, I tried the “cat /root/flag.txt” to print the flag, but didn’t work.

Then, I use “Strings” command and it worked.
I FOUND THE FLAG!
THM{AI_HACK_THE_******}
