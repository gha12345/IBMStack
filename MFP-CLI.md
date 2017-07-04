# IBM MobileFirst Platform Foundation Command Line Interface (CLI)

````bat

SYNTAX
     mfpdev <command> [options]

DESCRIPTION
     The IBM MobileFirst Platform Foundation Command Line Interface (CLI) is a 
     command-line for developing MobileFirst applications. The command-line can
     be used by itself, or in conjunction with the IBM MobileFirst Platform 
     Foundation Operations Console. Some functions are available from the 
     command-line only and not the console.
     
     You can run mfpdev commands in two modes: interactive mode and direct mode.
     In interactive mode, you enter the command without options, and you are 
     prompted for responses. In direct mode, you enter the full command, 
     including options, and prompts are not provided. When applicable, the
     prompts are context-sensitive to the target platform of the app, as 
     determined by the directory from which you run the command. Use the up and
     down arrow keys on your keyboard to move through the selections, and press
     the Enter key when the selection you want is highlighted and preceded by 
     a > character.
     
     For more information and a step-by-step example of using the CLI, see the 
     IBM Knowledge Center for your version of IBM MobileFirst Platform 
     Foundation at 
     
          https://www.ibm.com/support/knowledgecenter


ADAPTERS
     adapter build ... Builds a MobileFirst adapter
     adapter call .... Calls an adapter's procedure on the MobileFirst Server
     adapter create .. Creates a MobileFirst adapter
     adapter deploy .. Deploys a MobileFirst adapter
     adapter pull .... Pulls an adapter's configuration from the MobileFirst Server
     adapter push .... Pushes an adapter's configuration to the MobileFirst Server

APPLICATIONS
     app config ...... Configures application-specific settings.
     app preview ..... Previews your app.
     app pull ........ Pulls application configuration from a server
     app push ........ Pushes application configuration to a server
     app register .... Registers an application or applications to a server
     app webencrypt .. Encrypts a platform's 'www' folder in a Cordova project
     app webupdate ... Generates and deploys a .zip file of web resources to a MobileFirst Server.

GLOBAL
     config .......... Configures global preferences for the MobileFirst Platform Command Line Interface.
     info ............ Displays information about your environment.

SERVERS
     server add ...... Adds a new server definition.
     server clean .... Clean apps and adapters in an existing server.
     server console .. Opens the IBM MobileFirst Platform Operations Console.
     server edit ..... Edits an existing server profile.
     server info ..... Provides information for all servers or a specific server.
     server remove ... Removes an existing server profile.

COMMAND-LINE FLAGS/OPTIONS
      -v, --version .. Prints out this utility's version
      -d, --debug .... Debug mode produces debug log output
      -dd, --ddebug .. Debug mode produces verbose log output
      --no-color ..... Suppresses use of color in command output

EXAMPLES
      $ mfpdev app register

      Registers the application that resides in the current project directory
      on the default MobileFirst Server.

      $ mfpdev app pull Server1

      Pulls the application's configuration file from the MobileFirst Server
      whose profile is named Server1 to the local computer.

      $ mfpdev server add

      Invokes the interactive mode of the 'server add' command, to enable you to
      add a new MobileFirst Server profile. You are prompted for a new server
      profile name, URL, login credentials and other information about the
      server.

      $ mfpdev app preview ios -type mbs

      Displays a preview of the iOS version of a Cordova application in the
      Mobile Browser Simulator.


MORE INFORMATION
      For more detailed help on each command:

      $ mfpdev help <command>

````
