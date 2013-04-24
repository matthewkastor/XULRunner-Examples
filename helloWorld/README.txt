This example application was built and run with xulrunner 18.0.1 It should work with recent versions of xulrunner and continue to work with future versions of xulrunner but there are no guarantees. At any rate, the max version setting in application.ini is set to 200.* and the min version is set to 1.8 although I have absolutely no idea whether or not this works on all those past and future versions. Try it, if it works you're ready to go and if not you can rummage through the literature on mozilla developer network and make a helloworld application for whatever version xulrunner has gotten to (and give it to the new guys of course). :D


Now, if you are using xulrunner 18.0.1 the following information will work on windows for sure. If you're using other versions or operating systems rest of this information may or may not help much.

If you want to use the bat files to launch this application on XUL Runner you will need to adjust the paths in them to suit your system and copy helloWorld.exe into the same folder where xulrunner.exe is. Of course you can launch this app by calling <path to xulrunner>\xulrunner.exe --app application.ini from this directory but, you won't get the fancy icon and convenient clicky bat file. If you are using a different version of xulrunner you'll need to recreate helloWorld.exe using a copy of xulrunner-stub.exe that came with your version of xulrunner.

xulrunner-stub.exe comes with XUL Runner. Somewhere on mozilla's developer network I read the directions that the stub is a kind of proxy for xulrunner.exe, to enable us to give our applications a specific name and icon on windows. I don't remember how it finds xulrunner.exe exactly but I do know that if they're in the same directory the stub will launch xulrunner and pass any arguments to it.

All helloWorld.exe is, is the xulrunner-stub.exe with an application icon injected into it using resourcehacker. The application icon is easy to create using gimp, creating each layer of the image as the different sizes of icon, and exporting the image as an icon. Use the resource hacker to pull the appicon out of the exe and look at it in gimp. It's really easy to make.

http://angusj.com/resourcehacker/
http://www.gimp.org/tutorials/Creating_Icons/

You can also create shortcuts to the bat files and modify the shortcuts's properties so they'll use the icon from helloWorld.exe. You can specify that the bat file is to be launched minimized so it doesn't flash across the screen.

Have fun!


Kastor

☭ Hial Atropa!! ☭

