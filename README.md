::: {#page}
::: {#main .aui-page-panel}
::: {#main-header}
::: {#breadcrumb-section}
1.  [mahotest](index.html)
2.  [mahotest Home](mahotest-Home_258740839.html)
3.  [PSEAR Development (Copy)](258740842.html)
4.  [X \[archived\] PSEAR - Development Documentation
    (Copy)](258740846.html)
:::

# [ mahotest : (x) PSEAR - 1. MacBook Pro Environment Setup (Copy) ]{#title-text} {#title-heading .pagetitle}
:::

::: {#content .view}
::: {.page-metadata}
Created by [ Martin Hohenberg]{.author}, last modified on 2021-01-26
:::

::: {#main-content .wiki-content .group}
*~Derived\ from\ the [ Hybris\ Docs](https://www.secrz.de/confluence/pages/viewpage.action?pageId=105397505)~*

\

## Contents: {#id-(x)PSEAR-1.MacBookProEnvironmentSetup(Copy)-Contents: .title}

1.  **Homebrew**
2.  **wget**
3.  **JDK8 [*(JDK11 is also necessary, but must be downloaded from
    Oracle)*]{style="color: rgb(122,134,154);"}**
4.  **Git**
5.  **Docker**
6.  **Node**
7.  **Gradle**

\

## RocketChat MAC Community Support {#id-(x)PSEAR-1.MacBookProEnvironmentSetup(Copy)-RocketChatMACCommunitySupport}

For further questions feel free to join the RocketChat MAC Community
Channel: <https://chat.int.secrz.com/channel/macintosh_community>

\

Premise: Install homebrew and wget (Disconnect the VPN!)

\

1.  ### **Install Homebrew ** {#id-(x)PSEAR-1.MacBookProEnvironmentSetup(Copy)-InstallHomebrew}

    1.  Create the homebrew directory and download the software inside
        of it:

        ::: {.table-wrap}
          -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
          `mkdir homebrew && curl -L https:`{.java .plain style="text-align: left;"}`//github.com/Homebrew/brew/tarball/master | tar xz --strip 1 -C homebrew`{.java .comments style="text-align: left;"}
          -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
        :::

    2.  Move in your home directory (e.g. /Users/pirillo):

        ::: {.table-wrap}
          ------------------------------------------------
          `cd ~`{.java .plain style="text-align: left;"}
          ------------------------------------------------
        :::

    3.  Edit or create **.bash_profile** (e.g. vim ./.bash_profile)

    4.  Add the following line:

        ::: {.table-wrap}
          ---------------------------------------------------------------------------------------
          `export PATH=/Users/$USER/homebrew/bin:$PATH`{.java .plain style="text-align: left;"}
          ---------------------------------------------------------------------------------------
        :::

    5.  Save your **.bash_profile** file

    6.  Load the changes in your local environment by typing

        ::: {.table-wrap}
          ------------------------------------------------------------------
          `source ~/.bash_profile`{.java .plain style="text-align: left;"}
          ------------------------------------------------------------------
        :::

    7.  Check if **homebrew** is working by typing

        ::: {.table-wrap}
          ----------------------------------------------------------
          `brew --version`{.java .plain style="text-align: left;"}
          ----------------------------------------------------------
        :::

2.  ### **Install wget *(\~5/10min)* ** {#id-(x)PSEAR-1.MacBookProEnvironmentSetup(Copy)-Installwget(~5/10min) .auto-cursor-target}

    ::: {.table-wrap}
      -------------------------------------------------------------
      `brew install wget`{.java .plain style="text-align: left;"}
      -------------------------------------------------------------
    :::

3.  ### **Install JDK8** {#id-(x)PSEAR-1.MacBookProEnvironmentSetup(Copy)-InstallJDK8}

    1.  Open **Self Service**

    2.  Install **Oracle Java JDK**

4.  ### **Install Git ** {#id-(x)PSEAR-1.MacBookProEnvironmentSetup(Copy)-InstallGit}

    \
    Reconnect the VPN!

    1.  Open the terminal and digit

        ::: {.table-wrap}
          -----------------------------------------------
          `git`{.java .plain style="text-align: left;"}
          -----------------------------------------------
        :::

    2.  Then Apple will suggest you to install \"**command line
        tools**\". Accept.

    3.  Check if it is working

        ::: {.table-wrap}
          ---------------------------------------------------------
          `git --version`{.java .plain style="text-align: left;"}
          ---------------------------------------------------------
        :::

    4.  Setup your username and email

        ::: {.table-wrap}
          -----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
          `git config --global user.name `{.java .plain style="text-align: left;"}`"YourName YourSurname"`{.java .string style="text-align: left;"} `git config --global user.email mybeautiful.name`{.java .plain style="text-align: left;"}`@lidl`{.java .color1 style="text-align: left;"}`.com`{.java .plain style="text-align: left;"}
          -----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
        :::

5.  ### **Docker** {#id-(x)PSEAR-1.MacBookProEnvironmentSetup(Copy)-Docker style="text-align: left;"}

    Source

    Further Information available at: [Database Installation
    Guide](https://hub.docker.com/r/sath89/oracle-12c/){.external-link} & [Docker
    Commands
    Reference](https://docs.docker.com/engine/reference/commandline/cli/){.external-link}

    1.  Download Docker from Self Service

6.  ### **Node** {#id-(x)PSEAR-1.MacBookProEnvironmentSetup(Copy)-Node}

    \

    In the terminal type the following command to install Node.

    ::: {.code .panel .pdl style="border-width: 1px;"}
    ::: {.codeContent .panelContent .pdl}
    ``` {.syntaxhighlighter-pre syntaxhighlighter-params="brush: java; gutter: false; theme: Confluence" theme="Confluence"}
    brew install node
    ```
    :::
    :::

    If everything installed successfully then you can type in the
    following command in the terminal to check the Node and NPM version.

    ::: {.code .panel .pdl style="border-width: 1px;"}
    ::: {.codeContent .panelContent .pdl}
    ``` {.syntaxhighlighter-pre syntaxhighlighter-params="brush: java; gutter: false; theme: Confluence" theme="Confluence"}
    $ node -v
    v7.7.2
    $ npm -v
    4.1.2
    ```
    :::
    :::

    7\. Gradle

7.  ### **Gradle** {#id-(x)PSEAR-1.MacBookProEnvironmentSetup(Copy)-Gradle}

::: {.code .panel .pdl style="border-width: 1px;"}
::: {.codeContent .panelContent .pdl}
``` {.syntaxhighlighter-pre syntaxhighlighter-params="brush: java; gutter: false; theme: Confluence" theme="Confluence"}
brew install gradle
```
:::
:::
:::
:::
:::

::: {#footer role="contentinfo"}
::: {.section .footer-body}
Document generated by Confluence on 2021-01-26 08:43

::: {#footer-logo}
[Atlassian](http://www.atlassian.com/)
:::
:::
:::
:::
