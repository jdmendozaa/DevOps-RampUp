# Server configuration management

It’s time to revisit the scripts you wrote in the challenge [Scripting](scripting.md). In a traditional sysadmin world, usually, the configuration of servers (everything the server needs to work) are managed either manually or by a bunch of scripts that automate some processes. Imagine if one of those servers fails, our instinct would tell us to log in to that server, enter some commands, maybe change some configurations files, press some buttons or change one of those bash scripts we wrote. Great! the server is running again and now you can go home. Now imagine if you keep doing the same over and over; in the end, you will end up with a bunch of servers that everyone fears to touch because no one really knows how it works or how it’s configured. Also, you’ll find yourself making backups of those servers very often. That’s what we call **Snowflake servers** and we should do whatever it takes to prevent that to happen.

Fortunately, exists some tools that will help you to manage the configuration of your servers in an easier and more efficient way. Most of those tools will let you express the desired state of the system instead of a series of instructions or to achieve that state. The tool will do the necessary steps to convert the system from its current state to the state you specified.

---

In this challenge you’ll need to replicate the configurations you made in the scripting challenge using a configuration management tool:

1. **Research the available tools and pick one.** Each tool has its advantages and disadvantages so, explain why you made that decision.

2. Just like the Scripting challenge, **create the code to provision your instance** with everything the app needs to work but, in this case, using the tool you chose.

3. Remember that your instances are now in the cloud and they should be disposable, meaning you should be able to destroy and recreate them anytime you want. **Your implementation needs to able to detect if a new instance was created and configure it accordingly.**
