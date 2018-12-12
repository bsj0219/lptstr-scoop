
<p align="center"><img src="https://kiedtl.surge.sh/img/open-scoop.png" alt="Open, open, open Scoop"/></p>
<p align="center">
<b><a href="https://github.com/Kiedtl/open-scoop#whats-this">What's this?</a></b>
|
<b><a href="https://github.com/Kiedtl/open-scoop#installation">Installation</a></b>
|
<b><a href="https://github.com/Kiedtl/open-scoop#i-want-to-add-an-app">Add an app</a></b>
|
<b><a href="https://github.com/Kiedtl/open-scoop#list-of-application-currenly-in-the-bucket">List of apps</a></b>
|
<b><a href="https://github.com/Kiedtl/open-scoop#acknowledgments">Acknowledgments</a></b>
</p>

- - -
<p align="center"><a href="https://github.com/kiedtl/open-scoop"><img src="https://img.shields.io/github/languages/code-size/kiedtl/open-scoop.svg" alt="Code-Size" /></a>
<a href="https://github.com/kiedtl/open-scoop"><img src="https://img.shields.io/github/repo-size/kiedtl/open-scoop.svg" alt="Repository size" /></a>
<a href="https://github.com/kiedtl/open-scoop"><img src="https://img.shields.io/badge/apps-977-yellow.svg" alt="Apps in bucket" /></a>
 <a href="https://github.com/kiedtl/open-scoop"><img src="https://img.shields.io/badge/lines%20of%20code-34000%2B-yellow.svg" alt="Lines of code" /></a> <a href="https://travis-ci.org/Kiedtl/open-scoop"><img src="https://travis-ci.org/Kiedtl/open-scoop.svg?branch=master" alt="Travis-CI" /></a>
<a href="https://github.com/kiedtl/open-scoop/blob/master/LICENSE"><img src="https://img.shields.io/github/license/kiedtl/open-scoop.svg" alt="License" /></a>
</p><p align="center"><a href="http://spacemacs.org"><img src="https://cdn.rawgit.com/syl20bnr/spacemacs/442d025779da2f62fc86c2082703697714db6514/assets/spacemacs-badge.svg" /></a></p>
 
### What's this? 
This repository is a [Scoop](http://scoop.sh/) bucket for pretty much any Windows application. CLI-utilities, such as `genact`, `hyperfine`, `fd`, or `alacritty` are especially encouraged. Open-Scoop currently has about 975+ apps in the bucket, which means that adding the bucket can take longer that other buckets (less than two minutes for Scoop to clone the repository).

### Installation
Make sure you have Scoop installed:
```powershell
$ scoop which scoop
```

If Scoop is **not** installed, run the follwing code in Powershell (`powershell.exe` or `pwsh.exe`):
```powershell
$ Set-ExecutionPolicy RemoteSigned -Scope CurrentUser
$ Invoke-Expression (New-Object System.Net.WebClient).DownloadString("http://get.scoop.sh"
```

Then, add this repository as a bucket to Scoop:
```powershell
$ scoop bucket add openscoop http://github.com/kiedtl/open-scoop.git
$ scoop bucket list
```
If this bucket was correctly installed, you should see the following output:
```
$ scoop bucket list
extras
norsoft
...

openscoop
```
Now, try to install anything in this bucket:
```
$ scoop install genact alacritty process-explorer
$ scoop install pychess firefox 
$ scoop install cloc gitkraken chromium hyperfine sendemail
```

You can list all of the application in this bucket via the command-line
```powershell
$ scoop search
```

You can also search for an application in this repository without ever leaving the terminal by executing the following:
```powershell
$ scoop search <blah>
```

### I want to add an app!
No problem! Simply fork this repository and create a JSON file with the app manifest, using the guide [here](https://github.com/lukesampson/scoop/wiki/App-Manifests) here in the Scoop repository. 
Once you are done, just create a pull request describing which app you added, what it does, who is the creator of the app, and the latest version of the app. If possible, add the homepage and/or the repository link also. 

If you are adding a CLI utility that is hosted on GitHub and that is offered as a single, portable, standalone EXE, see the `genact.json` file for an example. 
If the application is an application on GitHub that need one or more files available on the internet to work properly, see the [Alacritty manifest](https://github.com/Kiedtl/open-scoop/blob/be9fb4a6b72ae6b436512dad6336f598ed154c64/alacritty.json#L22) for an example of how this can be worked around.

#### Requirements for adding an app
1. `Hello World` apps are not allowed.
2. The app added MUST be the full version of the app, not a trial version (although exceptions are made to this rule - see `sublime-text.json`).
3. There aren't any more requirements.

### List of application currenly in the bucket
**Note**: this list is outdated. See [Applist.md](APPLIST.md) for a complete, up-to-date listing of all application in this bucket.
```
   3rvx (2.9.2)
    7zip (18.05)
    ack (2.24)
    acmesharp (0.8.1.0)
    adb (28.0.1)
    advancedrenamer (3.84)
    ag (2.2.0-4-g1b06a9f)
    ahoy (2.0.0)
    aida64extreme (5.99)
    alacritty (0.2.3)
    allure (2.8.1)
    altools (1.0)
    ammonite (1.5.0)
    anaconda3 (5.3.1)
    android-sdk (4333796)
    android-studio (3.2.1.0)
    anki (2.1.6)
    annie (0.8.5)
    ant (1.10.5)
    antimicro (2.23)
    anydesk (4.2.3)
    apache-directory-studio (2.0.0-M14)
    apache-ivy (2.4.0)
    apache (2.4.37)
    apex (1.0.0-rc3)
    apngasm (3.0.0)
    appengine-go (1.9.70)
    archi (4.3)
    archwsl (18120900)
    arduino (1.8.8)
    aria2 (1.34.0-1)
    armclient (1.3)
    armor (0.4.12)
    artifact (1.0.1)
    assume-role (0.3.2)
    astrogrep (4.4.6)
    astyle (3.1)
    atom (1.33.0)
    atomicparsley (0.9.0)
    audacity (2.3.0)
    autohotkey-installer (1.1.30.01)
    autohotkey (1.1.30.01)
    autoit (3.3.14.5)
    awake (1.4.2)
    aws (1.16.72)
    axel (2.4)
    axis (1.4)
    azure-cli (2.0.52)
    azure-functions-core-tools (2.3.148)
    azure-ps (6.13.1.24243)
    azuredatastudio-insiders (1.2.4)
    azuredatastudio (1.2.4)
    baka-mplayer (2.0.4)
    bandizip (6.18)
    baretail (3.50a)
    bat (0.9.0)
    bazel (0.20.0)
    beatdrop (1.0.0.0)
    beyondcompare (4.2.8.23479)
    bfg (1.13.0)
    bitmessage (0.6.3.2)
    bitwarden-cli (1.6.0)
    bitwarden (1.11.2)
    bleachbit (2.0)
    blender (2.79b)
    blink1-tool (2.0.2)
    blink1control2 (2.2.0)
    blisk (10.1.262.114)
    bochs (2.6.9)
    boostnote (0.11.11)
    boot-clj (2.7.2)
    brackets (1.13)
    brave (0.26.0)
    brotli (1.0.7_1)
    buffalo (0.13.10)
    bulk-crap-uninstaller (4.12.1)
    busybox (2358-g25a1bcec7)
    bzip2 (1.0.6)
    cacert (2018-12-05)
    cacher (2.2.0)
    caddy (0.11.1)
    cake (0.30.0)
    calibre-normal (3.35.0)
    calibre (3.35.0)
    camunda-modeler (2.2.3)
    carnac (2.2.155)
    casperjs (1.1.4-2)
    ccat (1.1.0)
    ccleaner (5.50.6911)
    cdburnerxp (4.5.8.7041)
    cdrtools (3.01)
    championify (2.1.5)
    cheat-engine (6.8.1)
    chefdk (3.5.13)
    chrlauncher (2.5.3)
    chroma (0.6.0)
    chromedriver (2.45)
    chromium-dev-nosync (68.0.3424.0-r556419)
    chromium-dev (72.0.3615.0-r609145)
    chromium-nosync (67.0.3396.99-r550428)
    chromium (71.0.3578.80-r599034)
    clementine (1.3.1)
    clingo (5.3.0)
    clink (0.4.9)
    cloak (0.1.0)
    cloc (1.80)
    cloudfoundry-cli (6.41.0)
    cmake-rc (3.13.0-rc3)
    cmake (3.13.1)
    cmder-full (1.3.10)
    cmder (1.3.10)
    cmdow (1.4.8)
    cobalt (0.14.0)
    cockroachdb (2.1.2)
    codetrack (1.0.3.3)
    colortool (1810.02002)
    composer (1.8.0)
    concfg (0.2018.10.22)
    conemu (18.06.26)
    console2 (2.0.0.148)
    consolez (1.18.3.18143)
    consul (1.4.0)
    coretemp (1.12.1)
    coreutils (5.97.3)
    cowsay (0.2013.07.19)
    cppcheck (1.86)
    cpu-z (1.87)
    craft (april-2013)
    crystaldiskinfo (8.0.0)
    crystaldiskmark (6.0.2)
    cscope (15.8a)
    csvtosql (v0.1.1-alpha)
    ctags (5.8)
    cuetools (2.1.6)
    cura (3.6.0)
    curl (7.62.0_1)
    cutter (1.7.2)
    cygwin (2.895)
    darktable (2.4.4)
    dart-dev (2.2.0-dev.0.0)
    dart (2.1.0)
    darteditor (1.6.0)
    dartium-content-shell-dev (1.25.0-dev.6.0)
    dartium-content-shell (1.24.2)
    dartium-dev (1.25.0-dev.6.0)
    dartium (1.24.2)
    datamash (1.3)
    dbeaver (5.3.0)
    dbvis (10.0.16)
    dd (0.6beta3)
    ddev (1.4.1)
    ddu (18.0.0.4)
    deadlock (1.4)
    debugviewpp (1.8.0.34)
    defraggler (2.22.995)
    deluge (1.3.15)
    deno (0.2.2)
    dep (0.5.0)
    dependencies (1.9)
    depends (2.2)
    devd (0.8)
    devdocs (0.6.9)
    devrantron (1.5.4)
    dhcp-server (2.5.2)
    diff-pdf (2012-02-28)
    diffpdf (2.1.3)
    diffutils (3.5)
    dig (9.13.4)
    digdag (0.9.31)
    dirhash (1.7.1)
    discord-canary (0.0.224)
    discord-ptb (0.0.43)
    discord (0.0.301)
    dismplusplus (10.1.1000.80)
    ditto (3.21.258.0)
    dnsjumper (2.1)
    dnspy (5.0.0)
    docker-compose (1.23.2)
    docker-machine (0.16.0)
    docker-nightly (nightly)
    docker (18.09.0)
    dont-sleep (4.91)
    dopamine (1.5.14)
    dos2unix (7.4.0)
    dosbox (0.74-2)
    dotnet-sdk (2.2.100)
    dotnet (1.1.1)
    doublecmd (0.8.4)
    doxygen (1.8.14)
    draft (0.16.0)
    drone (1.0.4)
    ds4windows (1.5.18)
    duplicacy (2.1.2)
    eagleget-portable (2.0.4.80)
    easyrsa (3.0.5)
    easyserviceoptimizer (1.2)
    ec2-api-tools (1.7.3.0)
    echoargs (3.2)
    eclipse-android (4.6.3)
    eclipse-automotive (4.5.2)
    eclipse-committers (2018-09)
    eclipse-cpp (2018-09)
    eclipse-dsl (2018-09)
    eclipse-java (2018-09)
    eclipse-javascript (2018-09)
    eclipse-jee (2018-09)
    eclipse-mat (1.8.1.20180910)
    eclipse-modeling (2018-09)
    eclipse-parallel (2018-09)
    eclipse-php (2018-09)
    eclipse-platform (4.9-201809060745)
    eclipse-rcp (2018-09)
    eclipse-reporting (2018-09)
    eclipse-scout (2018-09)
    eclipse-sdk (4.9-201809060745)
    eclipse-testing (2018-09)
    edex-ui (1.1.2)
    edgedriver (6.17134)
    editorconfig (0.12.1)
    elasticsearch (6.5.2)
    elixir (1.7.4)
    elm (0.19.0)
    emacs (26.1)
    enpass (5.6.9)
    enso (0.4.2)
    erlang (21.2)
    etcher-cli (1.4.8)
    etcher (1.4.8)
    etlas (1.5.0.0)
    eventstore (4.1.1-hotfix1)
    everything (1.4.1.895)
    executor (0.99.27b)
    exercism-cli (3.0.11)
    exercism (3.0.11)
    exiftool (11.21)
    faas-cli (0.8.1)
    falcon-sql-client (4.0.0)
    far (30b5300)
    fastcopy (3.61)
    fastglacier (3.9.1)
    fciv (2.05)
    fd (7.2.0)
    ffmpeg-nightly (20181211-876ed08)
    ffmpeg (4.1)
    fiddler (5.0.20182.28034)
    figlet (1.0-go)
    file (5.03)
    filezilla (3.39.0)
    find-java (13)
    findutils (4.4.2)
    firefox-beta (nightly)
    firefox-developer (nightly)
    firefox-esr (60.4.0)
    firefox-nightly (nightly)
    firefox (63.0.3)
    firewallappblocker (1.6)
    flatc (1.10.0)
    flow (0.88.0)
    flutter (0.10.2)
    flux (4.84)
    flyway (5.2.4)
    fmedia (1.3)
    fnproject (0.5.35)
    fnr (1.8.1)
    fontforge (20170731-r2)
    foobar2000-encoders (2018-10-19)
    foobar2000 (1.4.1)
    force (0.25.0)
    forego (20180217041714)
    forge (2.2.0)
    format-factory (4.5.0.0)
    fossil (2.7)
    foxe (2.4.2)
    foxit-reader (9.3.0.10826)
    franz (5.0.0-beta.19)
    freac (1.0.32)
    freeclipboardviewer (3.0)
    freecommander (2018)
    freemind (1.0.1)
    fscapture (5.3)
    fsviewer (6.7)
    fzf (0.17.5)
    gawk (3.1.7)
    gcc-arm-none-eabi (7-2018-q2-update)
    gcc (8.1.0)
    gcloud (227.0.0)
    gdb (7.9.1)
    geany (1.33)
    geckodriver (0.23.0)
    geekuninstaller (1.4.5.134)
    genact (0.6.0)
    ghostscript (9.26)
    ghostwriter (1.7.1)
    ghq (0.8.0)
    gibo (2.1.0)
    gifcam (5.5)
    gifsicle (1.89)
    gimp (2.10.8)
    git-annex (7.20181205)
    git-crypt (0.6.0-701fb8e)
    git-istage (0.2.61)
    git-lfs (2.6.1)
    git-sizer (1.3.0)
    git-town (7.2.0)
    git-up (1.6.0)
    git-with-openssh (2.20.0.windows.1)
    git (2.20.0.windows.1)
    git19 (1.9.5-preview20150319)
    gitea (1.6.1)
    gitextensions (2.51.05)
    github (1.5.0)
    gitignore (0.2018.08.04)
    gitkraken (4.1.1)
    gitlab-runner (11.5.1)
    gitversion (4.0.0)
    glide (0.13.2)
    glogg (1.1.4)
    glslang-nightly (nightly)
    glslang (7.10.2984)
    gnirehtet (2.3)
    gnucash (3.2)
    gnupg (2.2.11)
    gnupg1 (1.4.23)
    go-ipfs (0.4.18)
    go (1.11.2)
    godot-mono (3.0.6)
    godot (3.0.6)
    gof (0.0.1)
    gogs (0.11.66)
    goldendict (1.5.0-RC2-311-g15062f7)
    google-java-format (1.6)
    gopass (1.8.3)
    gource (0.47)
    gow (0.8.0)
    gpg (2.2.11)
    gpg4win (3.1.5)
    gpu-z (2.16.0)
    gradle-bin (5.0)
    gradle (5.0)
    grafana (5.4.1)
    grails (3.3.9)
    graphicsgale (2.08.19)
    graphicsmagick-q16 (1.3.31)
    graphicsmagick-q8 (1.3.31)
    graphviz (2.38)
    greenshot (1.2.10.6)
    grep (2.5.4)
    groovy (2.5.4)
    groovyserv (1.2.0)
    guetzli (1.0.1)
    gzip (1.3.12)
    hack-font (1.6.0)
    hadoop-winutils (2.8.1)
    hain (0.6.6)
    HamMultiPlayer (0.116.37905.792)
    handbrake-cli (1.1.2)
    handbrake (1.1.2)
    harmony (0.9.1)
    hashcat (5.1.0)
    haskell (8.4.3)
    haskellx (7.8.3)
    haxe (3.4.7)
    heidisql (9.5)
    helm (2.12.0)
    helmfile (0.40.3)
    heroku-cli (nightly)
    hexchat (2.14.2)
    highlight (3.47)
    honeyview (5.31)
    hostsman (4.7.105)
    httrack (3.49.2)
    hub (2.6.1)
    hugo (0.52)
    hwinfo (5.92-3580)
    hwmonitor (1.38)
    hxd (2.1.0.0)
    hygen (1.6.4)
    hyper (2.0.0)
    hyperfine (1.4.0)
    ibmcloud-cli (0.12.1)
    iconv (1.14-3)
    idea-eap (183.4139.22)
    idea-ultimate-eap (183.4139.22)
    idea-ultimate (2018.3.1)
    idea (2018.3.1)
    idris (1.3.1)
    ie11webdriver (3.14.0)
    ilspy (3.2.0.3856)
    imageglass (5.5.7.26)
    imagemagick (7.0.8-16)
    imgburn (2.5.8.0)
    inadyn-mt (02.28.10)
    inboxer (1.2.1)
    influxdb (1.7.1)
    inkscape (0.92.3)
    inkscape32bit (0.92.3)
    innoextract (1.7)
    innounp (0.47)
    insect (5.0.0)
    insomnia (6.2.3)
    invoke-build (5.4.2)
    iographica (1.0.1)
    ios-webkit-debug-proxy (1.8.3)
    iperf3 (3.1.3)
    ipfilter-updater (3.0.0)
    ipscan (3.5.3)
    irfanview (4.51)
    jameica (2.8.2)
    jd-cmd (0.9.2)
    jd-gui (1.4.0)
    jdownloader (nightly)
    jetbrains-toolbox (1.12.4481)
    jfrog (1.22.1)
    jhead (3.00)
    jigsaw (2.2.6)
    jira (1.0.20)
    jitsi-meet-electron (1.1.1)
    jkrypto (4.4)
    joe (4.6)
    joplin (1.0.117)
    jpegview (1.0.37)
    jq (1.6)
    jruby (9.2.5.0)
    julia (1.0.2)
    just (0.3.13)
    kakaotalk (2.7.0.1858)
    kdenlive (18.08.2)
    kdiff3 (0.9.98)
    keepass (2.40)
    keepassxc (2.3.4)
    keeweb (1.6.3)
    keypirinha (2.23)
    keystore-explorer (5.4.1)
    kibana (6.5.2)
    kicad (5.0.1_4)
    kid3 (3.6.2)
    kindlegen (2.9)
    kitematic (0.17.6)
    kitty (0.70.0.7)
    knime (3.7.0)
    kompose (1.17.0)
    kotlin-native (0.9.3)
    kotlin (1.3.11)
    krita (4.1.5)
    ktlint (0.29.0)
    kubectl (1.13.0)
    lame (3.100)
    latex (2.9.6753)
    launchy (2.9.57)
    lazygit (0.5)
    lcow (v4.14.35-v0.3.9)
    ldap-admin (1.8.3)
    ldc (1.12.0)
    leet (2014.8.29)
    leiningen (2.8.1)
    less (530)
    lessmsi (1.6.3)
    lf (r8)
    libreoffice-fresh (6.1.3.2)
    libsndfile (1.0.28)
    libwebp (1.0.0)
    licecap (1.26)
    lightbulb (1.6.4.1)
    lightshot (nightly)
    lighttable (0.8.1)
    lighttpd (1.4.49-1)
    lili (2.9.4)
    lilypond (2.18.2)
    linqpad (nightly)
    linqpadless (1.1.0)
    listenmoeclient (2.0.0)
    llvm (7.0.0)
    lmms (1.1.3)
    ln (0.2018.08.04)
    lockhunter (3.2.3)
    logexpert (1.6.13)
    logstash (5.6.1)
    losslesscut (1.14.0)
    love (11.2)
    lua (5.1.5-52)
    lunacy (3.12)
    lxrunoffline (3.3.2)
    lynx (2.8.9rel.1)
    lzip (1.20)
    madvr (0.92.17)
    mailsend (1.19)
    make (4.2)
    makemkv (1.14.2)
    mancy (3.2.0)
    mariadb (10.3.11)
    maven (3.6.0)
    mc (4.8.19)
    MediaCreationTool (10.0.17763.1)
    mediainfo-gui (18.12)
    mediainfo (18.12)
    megasync (3.7.1.0)
    meld (3.18.3)
    mercurial (4.8.1)
    metastore (1.1.2-9-gdafa727)
    micro (1.4.1)
    microsip (3.19.8)
    mill (0.3.5)
    mingit-busybox (2.20.0.windows.1)
    mingit (2.20.0.windows.1)
    miniconda3 (4.5.11)
    minikube (0.31.0)
    minio-client (2018-12-05T22-59-07Z)
    minio (2018-12-06T01-27-43Z)
    minishift (1.28.0)
    minisign (0.8)
    mitmproxy (4.0.4)
    mkcert (1.1.2)
    mkvtoolnix (29.0.0)
    mls-software-openssh (7.9p1-1)
    mobaxterm (11.0)
    modd (0.7)
    monero (0.13.0.4)
    mongodb-compass-community (1.16.3)
    mongodb (4.0.4)
    mono (5.16.0.220)
    moonscript (0.5.0)
    mousejiggler (1.7.4)
    mozjpeg (3.3.1)
    mp3tag (2.91)
    mpc-be (1.5.2)
    mpc-hc-fork (1.8.3)
    mpc-hc (1.7.13)
    mpc-qt (18.08)
    mplayer (38117)
    mpv-git (20181202)
    mpv (2018-10-02)
    mqtt-spy (1.0.0)
    mremoteng (1.76.11.40527)
    msiafterburner (4.5.0)
    msmpi (9.0.1)
    msys (rev13)
    msys2 (20180531)
    mupdf (1.14.0)
    musescore (2.3.2)
    musicbee (3.2.6827)
    mysql-workbench (8.0.13)
    mysql (8.0.13)
    nano (2.5.3)
    naps2 (5.8.2)
    nasm (2.14)
    natural-docs (2.0.2)
    ncftpclient (3.2.6)
    neko (2.2.0)
    neofetch (5.0.0)
    neovim (0.3.1)
    netbeans (9.0)
    netcat (1.12)
    netlifyctl (0.4.0)
    nexusfont (2.6.2.1870)
    nginx (1.15.7)
    ngrok (4VmDzA7iaHb)
    nikto (2.1.5)
    nim (0.19.0)
    nimbleset (2.2.0.41590)
    nimbletext (2.9.1.36018)
    ninja (1.8.2)
    nircmd (2.81)
    nirlauncher (1.20.64)
    nmap (7.70)
    node-chakracore (10.13.0)
    node-compiler (1.5.0)
    nodejs-lts (10.14.1)
    nodejs (11.4.0)
    nomacs (3.12.1)
    notepad2-mod (4.2.25.998)
    notepad2 (4.2.25)
    notepadplusplus-pm (1.4.12)
    notepadplusplus (7.6)
    now-cli (12.1.11)
    nsis (3.03)
    nssm (2.24)
    nteract (0.12.3)
    nuget-package-explorer (5.0.116)
    nuget (4.8.1)
    nvm (1.1.7)
    nwjs-sdk (0.35.1)
    nwjs (0.35.1)
    obs-studio-small (21.1.2)
    obs-studio (22.0.2)
    ocenaudio (3.5.4)
    octave (4.4.1)
    oh-my-posh (2.0.230)
    omnisharp (1.32.8)
    onefetch (1.0.0)
    oneget (nightly)
    oni (0.3.6)
    openhab (2.3.0)
    openhardwaremonitor (0.8.0)
    openliberty (18.0.0.3)
    openresty (1.13.6.2)
    openshift-origin-client (3.11.0)
    openssh (7.6p1)
    openssl-slp (1.1.0j)
    openssl (1.1.1a_1)
    opentrack (2.3.10)
    openvpn (2.4.6-I602)
    opera (57.0.3098.91)
    optipng (0.7.7)
    orca (3.1.4000.1830)
    outlook-google-calendar-sync (2.7.7-alpha)
    oxipng (2.1.8)
    p4merge (152.131.2139)
    packer (1.3.3)
    paint.net (4.1.5)
    palemoon-portable (28.2.2)
    palemoon (28.2.2)
    pandoc-crossref (0.3.4.0)
    pandoc (2.5)
    papdesigner (2.2.0.8.04)
    patch (2.6.1)
    patheditor (1.0)
    pathod (4.0.4)
    pcem (14)
    pci-z (2.0-2017.07.01)
    pciutils (3.5.5)
    pcregrep (10.20)
    pdf2djvu (0.9.8)
    pdfsam (3.3.7)
    pdftk (2.02)
    peco (0.5.3)
    peerblock (1.1.691)
    pentaho-data-integration (8.2.0.0-342)
    perl (5.28.1.1)
    persepolis (3.1.0)
    pester (4.4.2)
    phantomjs (2.1.1)
    php-nts-xdebug (2.6.1-7.2)
    php-nts (7.2.13)
    php-xdebug (2.6.1-7.2)
    php (7.2.13)
    picard (2.0.4)
    picotorrent (0.15.0)
    pixie (4.1)
    pkg-config (0.26-1)
    plantuml (1.2018.13)
    png2html (1.1)
    png2jpeg (1.0.1.7)
    pngcrush (1.8.11)
    pngquant (2.12.1)
    poppler (0.68.0)
    portainer (1.19.2)
    posh-docker (0.7.0)
    posh-git (0.7.1)
    postgresql (11.1)
    postman (6.6.1)
    potrace (1.15)
    powerping (1.2.0)
    powertab (1.1.0)
    ppsspp (1.7.4)
    premake4 (4.4-b5)
    premake5 (5.0.0-alpha13)
    process-explorer (16.21)
    process-explorer64 (16.21)
    processhacker (2.39)
    procexp (16.21)
    procexp64 (16.21)
    prometheus (2.5.0)
    protobuf (3.6.1)
    proxifier-portable (3.42)
    psake (4.7.4)
    psgithub (2017.01.22)
    pshazz (0.2018.09.25)
    psiphon3 (136)
    PSPad (5.0.0)
    psutils (0.2018.08.04)
    pt (2.2.0)
    pup (0.4.0)
    puppet (5.5.8)
    purescript (0.12.1)
    putty (0.70)
    pwsafe (3.47.2)
    pwsh (6.1.1)
    px (2018-05-18)
    pycharm (2018.3.1)
    pychess (0.99.3)
    pypy2 (6.0.0)
    python-exp (3.5.2)
    python (3.7.1)
    python27 (2.7.15)
    python35 (3.5.4)
    qaac (2.68)
    qbittorrent (4.1.4)
    qemu (3.1.0-rc3)
    qnapi (0.2.3)
    qpdf (8.2.1)
    qrencode (3.4.4)
    quicklook (3.6.4)
    quiterss (0.18.12)
    qutebrowser (1.5.2)
    r (3.5.1)
    rabbitmq (3.7.9)
    rabbitmqadmin (3.7.9)
    racket (7.1)
    radare2 (3.1.3)
    ragel (6.9)
    rainmeter (4.2.0.3111)
    rambox-pro (1.0.8)
    rambox (0.6.3)
    rancher-compose (0.12.5)
    rapidee (937)
    rcedit (1.1.1)
    rclone (1.45)
    reaper (5.963)
    recuva (1.53.1087)
    red (0.6.4)
    redis (3.2.100)
    renderdoc (1.2)
    reshade (4.0.2)
    resharper-clt (2018.2.3)
    resource-hacker (5.1.6)
    restic (0.9.3)
    rethinkdb (2.3.6)
    retroarch (1.7.5)
    ripgrep (0.10.0)
    ripme (1.7.72)
    rktools2k3 (1.0)
    robo3t (1.2.1)
    rstudio (1.1.463)
    rtmpdump (2.3)
    ruby (2.4.5-1)
    rufus (3.4)
    runat (0.2018.08.04)
    rust-msvc-nightly (nightly)
    rust-msvc (1.30.1)
    rust-nightly (nightly)
    rust (1.30.1)
    rustup (1.16.0)
    rxrepl (1.5)
    s (0.5.13)
    s3deploy (2.2.0)
    sabnzbd (2.3.5)
    sacad (2.1.7)
    sandman (1.9.2)
    sass (1.15.2)
    say (0.2018.08.04)
    sbcl (1.4.14)
    sbt (1.2.7)
    scala (2.12.8)
    scallion (2.1)
    scholdoc (0.1.3)
    scons (3.0.1)
    scrcpy (1.5)
    screentogif (2.14.1)
    scriptcs (0.17.1)
    sdl2 (2.0.7)
    sed (4.2.1)
    selenium (3.141.59)
    sendemail (156)
    seqcli (5.0.165)
    serve (0.2.1)
    servicebusexplorer (4.0.110)
    sfk (1.9.3.4)
    shadowsocks (4.1.2)
    shadowsocksr-csharp (4.9.0)
    sharex (12.3.1)
    sharpkeys (3.8)
    shasum (0.2018.08.04)
    shellcheck (0.6.0)
    shim (0.2013.11.19)
    shinjiru (3.3.2)
    signal (1.19.0)
    simplewall (2.3.10)
    skaffold (0.19.0)
    slack (3.3.3)
    sliksvn (1.9.7)
    smartmontools (6.6-1)
    smartty (3.1)
    snaketail (1.9.4)
    snipaste (1.16.2)
    soapui (5.4.0)
    solidity (0.5.1)
    sonarqube (7.4)
    soulseekqt (2017-2-20)
    sourcetree (3.0.12)
    SpaceSniffer (1.3.0.2)
    spark (2.4.0)
    speccy (1.32.740)
    speedcrunch (0.12)
    speedfan (4.52)
    speedyfox (2.0.25)
    springboot (2.1.1)
    spytify (1.1.3.1)
    sqlite (3.26.0)
    sqlitebrowser (3.10.1)
    sqlitestudio (3.2.1)
    sqlopsstudio (0.33.7)
    squashfs-tools (43)
    srvman (1.0)
    ssd-z (16.09.09)
    ssh-copy-id (2015-03-22)
    sslscan (1.11.11)
    stack (1.9.3)
    station (1.31.3)
    steam-library-manager (1.5.0.12)
    steam (nightly)
    steamcmd (1532461524)
    stone-soup-tiles (0.22.1)
    stone-soup (0.22.1)
    storageexplorer (1.5.0)
    streamlink (0.14.2)
    strokesplus-portable (2.8.6.4)
    sts (3.9.6)
    stunnel (5.49)
    sublime-merge (1097)
    sublime-text (3176)
    subtitleedit (3.5.7)
    sudo (0.2018.08.04)
    sumatrapdf (3.1.2)
    sunsetscreen (1.30)
    svcat (0.1.38)
    svtplay-dl (2.1)
    sweethome3d (6.0)
    swig (3.0.12)
    syncany-cli (0.4.9)
    syncbackpro (8.5.97.0)
    syncthing (0.14.54)
    synctrayzor (1.1.22)
    sysinternals (July.5.2018)
    taiga (1.3.1)
    tar (1.23)
    task (2.2.1)
    tcc (0.9.26)
    tcpipmanager (4.1.1)
    teamspeak3 (3.2.3)
    teamviewer (14.0.13880)
    telegram (1.5.1)
    telnet (msys-inetutils-1.7-1)
    terminals (4.0.1)
    terminus (1.0.65)
    terraform (0.11.10)
    terragrunt (0.17.3)
    tesseract (4.0.0.20181030)
    texmaker (5.0.3)
    texstudio (2.12.14)
    textadept (10.2)
    texteditoranywhere (2.01)
    thrift (0.11.0)
    thunderbird (60.3.3)
    tidy (5.6.0)
    time (0.2018.08.04)
    todolist (7.1.5.0)
    tomcat (9.0.12)
    tor-browser (8.0.4)
    tor-expert (0.3.4.9)
    tortoisemerge (1.6.7)
    tortoisesvn (1.11.0.28416)
    totalcommander (9.21a)
    touch (0.2018.08.04)
    traefik (1.7.5)
    transmission-cli (2.94)
    transmission (2.94)
    tremulous (1.3.0-alpha.0.13)
    trid (2.24-18.12.11)
    tunnel (0.2.12)
    tup (0.7.8)
    UIforETW (1.50)
    unar (1.8.1)
    unbound (1.8.3)
    uncap (0.2.2)
    uncrustify (0.68.1)
    unetbootin (661)
    ungoogled-chromium (67.0.3396.87-3)
    universalpausebutton (1.0.3)
    unlocker (1.9.0)
    unrar (5.61)
    unzip (6.00)
    up (0.8.1)
    upx (3.95)
    usql (0.7.0)
    util-linux-ng (2.14.1)
    vagrant (2.2.2)
    vault (1.0.0)
    vbindiff (3.0-beta5)
    vcredist (14.10.25008)
    vcredist2008 (9.0.30729)
    vcredist2010 (10.0.40219)
    vcredist2012 (11.0.61030)
    vcredist2013 (12.0.40660)
    vcredist2015 (14.0.24215)
    vcredist2017 (14.10.25008)
    vcxsrv (1.20.1.4)
    vifm (0.10)
    vim (8.1.0576)
    vimtutor (0.2018.08.04)
    visual-arm-emulator (1.27)
    visualc (16.00.30319.01)
    vivaldi (2.1.1337.51)
    vlc (3.0.4)
    vncviewer (6.18.907)
    vnote (2.1)
    vott (1.7.1)
    vscode-insiders-portable (nightly)
    vscode-insiders (nightly)
    vscode-portable (1.29.1)
    vscode (1.29.1)
    vswhere (2.5.2)
    warp (0.3.0)
    watchexec (1.9.2)
    watchman-nightly (nightly)
    wavebox (4.5.5)
    webpicmd (4.5)
    webstorm (2018.3.1)
    webtorrent (0.20.0)
    wget (1.20)
    whatsapp (0.3.1649)
    which (2.20)
    wifi-manager (0.2)
    win-acme (1.9.12.2)
    win-portacle (1.2c)
    win32-disk-imager (1.0.0)
    win32-openssh (7.7.2.0p1-Beta)
    winbox (3.18)
    wincdemu (4.0)
    wincompose (0.8.2)
    windirstat (1.1.2)
    windows-application-driver (1.1)
    winfile-original (10.0)
    winfile (10.0.1806.1)
    winmerge (2.16.0)
    winmerge2011 (0.2011.008.313)
    winpython (3.6.7.0)
    winrar (5.61)
    winscp (5.13.5)
    winyl (3.3.1)
    wireshark (2.6.5)
    wixtoolset (3.11.1)
    wiztree (3.26)
    wkhtmltopdf (0.12.5-1)
    wox (1.3.524)
    write (1.0b8.4)
    wsltty (1.9.5)
    wurl (1.0.1)
    wuzz (0.4.0)
    wxhexeditor (0.24)
    wyam (2.1.0)
    x264-10bit (2851)
    x264 (2935)
    x64dbg (2018-11-27_12-40)
    xdelta (3.1.0)
    xdman (7.2.8)
    xmake (2.2.3)
    xmedia-recode (3.4.4.8)
    xmind8 (3.7.8)
    xming (6.9.0.31)
    xmllint (2.9.3)
    xmlstarlet (1.6.1)
    xmousebuttoncontrol (2.17)
    xsv (0.13.0)
    xx-net (3.12.11)
    xyplorer (17.40.0100)
    xz (5.2.4)
    yara (3.8.1)
    yarn (1.12.3)
    yasm (1.3.0)
    yatqa (3.9.5)
    youtube-dl-gui (0.4)
    youtube-dl (2018.12.09)
    yubico-piv-tool (1.6.2)
    yubikey-manager-qt (0.5.2)
    yubikey-personalization-gui (3.1.25)
    yubikey-personalization (1.19.0)
    yubikey-piv-manager (1.4.2)
    zeal (0.6.1)
    zeppelin (0.8.0)
    zeronet (0.6.4)
    ziglang (0.3.0)
    zip (3.0)
    zlocation (1.1.0)
    zola (0.5.0)
    zookeeper (3.4.13)
    zstd (1.3.7)

'versions' bucket:
    7zip-beta (18.03)
    7zip-zstd (17.01-v1.3.2-R1)
    ant19 (1.9.13)
    apache24 (2.4.37)
    atom18 (1.8.0-beta3)
    chromium-dev70 (70.0.3518.0-r581881)
    elasticsearch1 (1.7.6)
    elasticsearch2 (2.4.6)
    elasticsearch5 (5.6.13)
    flow030 (v0.30.0)
    flow031 (v0.31.0)
    gcc45 (4.5.2)
    gradle4 (4.10.3)
    hub23 (2.3.0-pre9)
    love0.10.0 (0.10.0)
    love0.10.1 (0.10.1)
    love0.10.2 (0.10.2)
    love0.6.2 (0.6.2)
    love0.7.0 (0.7.0)
    love0.7.1 (0.7.1)
    love0.7.2 (0.7.2)
    love0.8.0 (0.8.0)
    love0.9.0 (0.9.0)
    love0.9.1 (0.9.1)
    love0.9.2 (0.9.2)
    lynx283 (2.8.3)
    mongodb34 (3.4-latest)
    mysql56 (5.6.42)
    mysql57 (5.7.24)
    nodejs010 (0.10.48)
    nodejs012 (0.12.18)
    nodejs4 (4.9.1)
    nodejs6 (6.15.1)
    nodejs7 (7.10.1)
    nodejs8 (8.14.0)
    nodejs9 (9.11.2)
    nuget3 (3.5.0)
    openssl10x (1.0.2q)
    phantomjs19 (1.9.8)
    php54 (5.4.45)
    php55-xdebug (2.5.5-5.5)
    php55 (5.5.38)
    php56-xdebug (2.5.5-5.6)
    php56 (5.6.39)
    php70-xdebug (2.6.1-7.0)
    php70 (7.0.33)
    php71-xdebug (2.6.1-7.1)
    php71 (7.1.25)
    php72-xdebug (2.6.1-7.2)
    php72 (7.2.13)
    postgresql10 (10.5)
    premake4 (4.4-b5)
    premake5 (5.0.0-alpha13)
    python-beta (3.7.0)
    python27 (2.7.15)
    python35 (3.5.4)
    python36 (3.6.7)
    ruby19 (1.9.3-p551)
    sbt0.13 (0.13.16)
    springboot15 (1.5.18)
    tesseract3 (3.05.02-20180621)
    tesseract4 (4.0.0.20181030)
    tomcat6 (6.0.53)
    tomcat7 (7.0.90)
    tomcat80 (8.0.53)
    tomcat85 (8.5.33)
    zip-beta (3.1d26)
```

### Acknowledgments
Lots of thanks to the maintainers of the Scoop Extras bucket and the 
Scoop repository, from where I stole a lot of things.
### List of apps in bucket
---
Automatically generated by the bin/build.ps1 script

| Name | Version | Homepage |
| ---- | ------- | -------- |
| 3rvx | 2.9.2 | [https://3rvx.com/](https://3rvx.com/) |
| 7zip | 18.05 | [http://www.7-zip.org/](http://www.7-zip.org/) |
| ack | 2.24 | [https://beyondgrep.com/](https://beyondgrep.com/) |
| acmesharp | 0.8.1.0 | [https://github.com/ebekker/ACMESharp](https://github.com/ebekker/ACMESharp) |
| adb | 28.0.1 | [https://developer.android.com/studio/releases/platform-tools.html](https://developer.android.com/studio/releases/platform-tools.html) |
| advancedrenamer | 3.84 | [https://www.advancedrenamer.com](https://www.advancedrenamer.com) |
| ag | 2.2.0-4-g1b06a9f | [https://geoff.greer.fm/ag/](https://geoff.greer.fm/ag/) |
| ahoy | 2.0.0 | [http://ahoycli.com](http://ahoycli.com) |
| aida64extreme | 5.99 | [https://www.aida64.com](https://www.aida64.com) |
| alacritty | 0.2.3 | [https://github.com/jwilm/alacritty/releases](https://github.com/jwilm/alacritty/releases) |
| allure | 2.8.1 | [https://github.com/allure-framework/allure2](https://github.com/allure-framework/allure2) |
| altools | 1.0 | [https://www.microsoft.com/en-us/download/details.aspx?id=18465](https://www.microsoft.com/en-us/download/details.aspx?id=18465) |
| ammonite | 1.5.0 | [http://ammonite.io](http://ammonite.io) |
| anaconda3 | 5.3.1 | [https://www.anaconda.com/](https://www.anaconda.com/) |
| android-sdk | 4333796 | [https://developer.android.com/studio/](https://developer.android.com/studio/) |
| android-studio | 3.2.1.0 | [https://developer.android.com/studio/](https://developer.android.com/studio/) |
| anki | 2.1.6 | [https://apps.ankiweb.net/](https://apps.ankiweb.net/) |
| annie | 0.8.5 | [https://github.com/iawia002/annie](https://github.com/iawia002/annie) |
| ant | 1.10.5 | [https://ant.apache.org/](https://ant.apache.org/) |
| antimicro | 2.23 | [https://github.com/AntiMicro/antimicro](https://github.com/AntiMicro/antimicro) |
| anydesk | 4.2.3 | [https://anydesk.com/](https://anydesk.com/) |
| apache-directory-studio | 2.0.0-M14 | [http://directory.apache.org/studio/](http://directory.apache.org/studio/) |
| apache-ivy | 2.4.0 | [https://ant.apache.org/ivy/index.html](https://ant.apache.org/ivy/index.html) |
| apache | 2.4.37 | [https://www.apachelounge.com](https://www.apachelounge.com) |
| apex | 1.0.0-rc3 | [http://apex.run/](http://apex.run/) |
| apngasm | 3.0.0 | [https://github.com/apngasm/apngasm](https://github.com/apngasm/apngasm) |
| appengine-go | 1.9.70 | [https://developers.google.com/appengine/](https://developers.google.com/appengine/) |
| archi | 4.3.1 | [https://www.archimatetool.com/](https://www.archimatetool.com/) |
| archwsl | 18120900 | [https://github.com/yuk7/ArchWSL/](https://github.com/yuk7/ArchWSL/) |
| arduino | 1.8.8 | [https://www.arduino.cc/](https://www.arduino.cc/) |
| aria2 | 1.34.0-1 | [https://aria2.github.io/](https://aria2.github.io/) |
| armclient | 1.3 | [https://github.com/projectkudu/ARMClient](https://github.com/projectkudu/ARMClient) |
| armor | 0.4.12 | [https://github.com/labstack/armor](https://github.com/labstack/armor) |
| artifact | 1.0.1 | [https://github.com/vitiral/artifact](https://github.com/vitiral/artifact) |
| assume-role | 0.3.2 | [https://github.com/remind101/assume-role](https://github.com/remind101/assume-role) |
| astrogrep | 4.4.6 | [http://astrogrep.sourceforge.net/](http://astrogrep.sourceforge.net/) |
| astyle | 3.1 | [http://astyle.sourceforge.net/](http://astyle.sourceforge.net/) |
| atom | 1.33.0 | [https://atom.io/](https://atom.io/) |
| atomicparsley | 0.9.0 | [http://atomicparsley.sourceforge.net/](http://atomicparsley.sourceforge.net/) |
| audacity | 2.3.0 | [https://www.audacityteam.org/](https://www.audacityteam.org/) |
| autohotkey-installer | 1.1.30.01 | [https://www.autohotkey.com/](https://www.autohotkey.com/) |
| autohotkey | 1.1.30.01 | [https://www.autohotkey.com/](https://www.autohotkey.com/) |
| autoit | 3.3.14.5 | [https://www.autoitscript.com/site/autoit/](https://www.autoitscript.com/site/autoit/) |
| awake | 1.4.2 | [https://github.com/gdegeneve/Awake](https://github.com/gdegeneve/Awake) |
| aws | 1.16.73 | [https://aws.amazon.com/cli/](https://aws.amazon.com/cli/) |
| axel | 2.4 | [https://github.com/ghuntley/cygwin-axel/](https://github.com/ghuntley/cygwin-axel/) |
| axis | 1.4 | [https://axis.apache.org/](https://axis.apache.org/) |
| azure-cli | 2.0.52 | [https://aka.ms/cli](https://aka.ms/cli) |
| azure-functions-core-tools | 2.3.148 | [https://github.com/Azure/azure-functions-core-tools](https://github.com/Azure/azure-functions-core-tools) |
| azure-ps | 6.13.1.24243 | [https://aka.ms/azpsdocs](https://aka.ms/azpsdocs) |
| azuredatastudio-insiders | 1.2.4 | [https://docs.microsoft.com/en-us/sql/azure-data-studio](https://docs.microsoft.com/en-us/sql/azure-data-studio) |
| azuredatastudio | 1.2.4 | [https://docs.microsoft.com/en-us/sql/azure-data-studio](https://docs.microsoft.com/en-us/sql/azure-data-studio) |
| baka-mplayer | 2.0.4 | [http://bakamplayer.u8sand.net/](http://bakamplayer.u8sand.net/) |
| bandizip | 6.18 | [http://www.bandisoft.com/bandizip/](http://www.bandisoft.com/bandizip/) |
| baretail | 3.50a | [https://www.baremetalsoft.com/baretail/](https://www.baremetalsoft.com/baretail/) |
| bat | 0.9.0 | [https://github.com/sharkdp/bat](https://github.com/sharkdp/bat) |
| bazel | 0.20.0 | [https://bazel.build](https://bazel.build) |
| beatdrop | 1.0.0.0 | [https://github.com/mvsoft74/BeatDrop](https://github.com/mvsoft74/BeatDrop) |
| beyondcompare | 4.2.8.23479 | [https://www.scootersoftware.com](https://www.scootersoftware.com) |
| bfg | 1.13.0 | [https://rtyley.github.io/bfg-repo-cleaner/](https://rtyley.github.io/bfg-repo-cleaner/) |
| bitmessage | 0.6.3.2 | [https://bitmessage.org/](https://bitmessage.org/) |
| bitwarden-cli | 1.6.0 | [https://bitwarden.com/](https://bitwarden.com/) |
| bitwarden | 1.11.2 | [https://bitwarden.com/](https://bitwarden.com/) |
| bleachbit | 2.0 | [https://www.bleachbit.org/](https://www.bleachbit.org/) |
| blender | 2.79b | [https://www.blender.org/](https://www.blender.org/) |
| blink1-tool | 2.0.2 | [https://blink1.thingm.com/](https://blink1.thingm.com/) |
| blink1control2 | 2.2.1 | [https://blink1.thingm.com/](https://blink1.thingm.com/) |
| blisk | 10.1.262.114 | [https://blisk.io/](https://blisk.io/) |
| bochs | 2.6.9 | [http://bochs.sourceforge.net/](http://bochs.sourceforge.net/) |
| boostnote | 0.11.11 | [https://boostnote.io/](https://boostnote.io/) |
| boot-clj | 2.7.2 | [https://github.com/boot-clj/boot](https://github.com/boot-clj/boot) |
| brackets | 1.13 | [http://brackets.io/](http://brackets.io/) |
| brave | 0.26.0 | [https://brave.com](https://brave.com) |
| brotli | 1.0.7 | [https://brotli.org/](https://brotli.org/) |
| buffalo | 0.13.10 | [https://gobuffalo.io](https://gobuffalo.io) |
| bulk-crap-uninstaller | 4.12.1 | [http://klocmansoftware.weebly.com/](http://klocmansoftware.weebly.com/) |
| busybox | 2358-g25a1bcec7 | [https://frippery.org/busybox](https://frippery.org/busybox) |
| bzip2 | 1.0.6 | [https://github.com/philr/bzip2-windows](https://github.com/philr/bzip2-windows) |
| cacert | 2018-12-05 | [https://curl.haxx.se/docs/caextract.html](https://curl.haxx.se/docs/caextract.html) |
| cacher | 2.2.0 | [https://www.cacher.io/](https://www.cacher.io/) |
| caddy | 0.11.1 | [https://caddyserver.com](https://caddyserver.com) |
| cake | 0.30.0 | [https://cakebuild.net/](https://cakebuild.net/) |
| calibre-normal | 3.35.0 | [https://calibre-ebook.com/](https://calibre-ebook.com/) |
| calibre | 3.35.0 | [https://calibre-ebook.com/](https://calibre-ebook.com/) |
| camunda-modeler | 2.2.3 | [https://camunda.org/download/modeler/](https://camunda.org/download/modeler/) |
| carnac | 2.2.155 | [http://carnackeys.com/](http://carnackeys.com/) |
| casperjs | 1.1.4-2 | [http://casperjs.org/](http://casperjs.org/) |
| ccat | 1.1.0 | [https://github.com/jingweno/ccat](https://github.com/jingweno/ccat) |
| ccleaner | 5.50.6911 | [https://www.piriform.com/ccleaner](https://www.piriform.com/ccleaner) |
| cdburnerxp | 4.5.8.7041 | [https://cdburnerxp.se/](https://cdburnerxp.se/) |
| cdrtools | 3.01 | [https://sourceforge.net/projects/tumagcc/](https://sourceforge.net/projects/tumagcc/) |
| championify | 2.1.5 | [https://github.com/dustinblackman/Championify](https://github.com/dustinblackman/Championify) |
| cheat-engine | 6.8.1 | [https://cheatengine.org/index.php](https://cheatengine.org/index.php) |
| chefdk | 3.5.13 | [https://chef.io](https://chef.io) |
| chrlauncher | 2.5.3 | [https://www.henrypp.org/product/chrlauncher](https://www.henrypp.org/product/chrlauncher) |
| chroma | 0.6.0 | [https://github.com/alecthomas/chroma](https://github.com/alecthomas/chroma) |
| chromedriver | 2.45 | [https://sites.google.com/a/chromium.org/chromedriver/](https://sites.google.com/a/chromium.org/chromedriver/) |
| chromium-dev-nosync | 68.0.3424.0-r556419 | [https://www.chromium.org](https://www.chromium.org) |
| chromium-dev | 72.0.3615.0-r609145 | [https://www.chromium.org](https://www.chromium.org) |
| chromium-nosync | 67.0.3396.99-r550428 | [https://www.chromium.org](https://www.chromium.org) |
| chromium | 71.0.3578.80-r599034 | [https://www.chromium.org](https://www.chromium.org) |
| clementine | 1.3.1 | [https://www.clementine-player.org/](https://www.clementine-player.org/) |
| clingo | 5.3.0 | [https://potassco.org/clingo/](https://potassco.org/clingo/) |
| clink | 0.4.9 | [https://mridgers.github.io/clink/](https://mridgers.github.io/clink/) |
| cloak | 0.1.0 | [https://github.com/evansmurithi/cloak](https://github.com/evansmurithi/cloak) |
| cloc | 1.70 | [https://github.com/AlDanial/cloc](https://github.com/AlDanial/cloc) |
| cloudfoundry-cli | 6.41.0 | [https://github.com/cloudfoundry/cli/](https://github.com/cloudfoundry/cli/) |
| cmake-rc | 3.13.0-rc3 | [https://cmake.org/](https://cmake.org/) |
| cmake | 3.13.1 | [https://cmake.org/](https://cmake.org/) |
| cmder-full | 1.3.10 | [http://cmder.net](http://cmder.net) |
| cmder | 1.3.10 | [http://cmder.net](http://cmder.net) |
| cmdow | 1.4.8 | [https://ritchielawrence.github.io/cmdow/](https://ritchielawrence.github.io/cmdow/) |
| cobalt | 0.14.0 | [https://cobalt-org.github.io/](https://cobalt-org.github.io/) |
| cockroachdb | 2.1.2 | [https://www.cockroachlabs.com/](https://www.cockroachlabs.com/) |
| codetrack | 1.0.3.3 | [http://www.getcodetrack.com](http://www.getcodetrack.com) |
| colortool | 1810.02002 | [https://github.com/Microsoft/Console/tree/master/tools/ColorTool](https://github.com/Microsoft/Console/tree/master/tools/ColorTool) |
| composer | 1.8.0 | [https://getcomposer.org/](https://getcomposer.org/) |
| concfg | 0.2018.10.22 | [https://github.com/lukesampson/concfg](https://github.com/lukesampson/concfg) |
| conemu | 18.06.26 | [https://conemu.github.io/](https://conemu.github.io/) |
| console2 | 2.0.0.148 | [https://sourceforge.net/projects/console/](https://sourceforge.net/projects/console/) |
| consolez | 1.18.3.18143 | [https://github.com/cbucher/console](https://github.com/cbucher/console) |
| consul | 1.4.0 | [https://www.consul.io](https://www.consul.io) |
| coretemp | 1.12.1 | [http://www.alcpu.com/CoreTemp/](http://www.alcpu.com/CoreTemp/) |
| coreutils | 5.97.3 | [http://www.mingw.org/wiki/msys](http://www.mingw.org/wiki/msys) |
| cowsay | 0.2013.07.19 | [https://github.com/lukesampson/cowsay-psh](https://github.com/lukesampson/cowsay-psh) |
| cppcheck | 1.86 | [http://cppcheck.sourceforge.net/](http://cppcheck.sourceforge.net/) |
| cpu-z | 1.87 | [https://www.cpuid.com/softwares/cpu-z.html](https://www.cpuid.com/softwares/cpu-z.html) |
| craft | april-2013 | [https://www.michaelfogleman.com/projects/craft/](https://www.michaelfogleman.com/projects/craft/) |
| crystaldiskinfo | 8.0.0 | [https://osdn.net/projects/crystaldiskinfo/](https://osdn.net/projects/crystaldiskinfo/) |
| crystaldiskmark | 6.0.2 | [https://osdn.net/projects/crystaldiskmark/](https://osdn.net/projects/crystaldiskmark/) |
| cscope | 15.8a | [http://cscope.sourceforge.net/](http://cscope.sourceforge.net/) |
| csvtosql | v0.1.1-alpha | [https://github.com/deevus/CsvToSql](https://github.com/deevus/CsvToSql) |
| ctags | 5.8 | [http://ctags.sourceforge.net/](http://ctags.sourceforge.net/) |
| cuetools | 2.1.6 | [http://cue.tools/wiki/Main_Page](http://cue.tools/wiki/Main_Page) |
| cura | 3.6.0 | [https://ultimaker.com/en/products/ultimaker-cura-software](https://ultimaker.com/en/products/ultimaker-cura-software) |
| curl | 7.63.0 | [https://curl.haxx.se/](https://curl.haxx.se/) |
| cutter | 1.7.2 | [https://github.com/radareorg/cutter](https://github.com/radareorg/cutter) |
| cygwin | 2.895 | [https://cygwin.com/](https://cygwin.com/) |
| darktable | 2.4.4 | [https://www.darktable.org/](https://www.darktable.org/) |
| dart-dev | 2.2.0-dev.0.0 | [https://www.dartlang.org/](https://www.dartlang.org/) |
| dart | 2.1.0 | [https://www.dartlang.org/](https://www.dartlang.org/) |
| darteditor | 1.6.0 | [https://www.dartlang.org](https://www.dartlang.org) |
| dartium-content-shell-dev | 1.25.0-dev.6.0 | [https://www.dartlang.org/](https://www.dartlang.org/) |
| dartium-content-shell | 1.24.2 | [https://www.dartlang.org/](https://www.dartlang.org/) |
| dartium-dev | 1.25.0-dev.6.0 | [https://www.dartlang.org/](https://www.dartlang.org/) |
| dartium | 1.24.2 | [https://www.dartlang.org/](https://www.dartlang.org/) |
| datamash | 1.3 | [https://www.gnu.org/software/datamash/](https://www.gnu.org/software/datamash/) |
| dbeaver | 5.3.0 | [https://dbeaver.io/](https://dbeaver.io/) |
| dbvis | 10.0.16 | [https://www.dbvis.com/](https://www.dbvis.com/) |
| dd | 0.6beta3 | [http://www.chrysocome.net/dd](http://www.chrysocome.net/dd) |
| ddev | 1.4.1 | [https://ddev.readthedocs.io/en/latest/](https://ddev.readthedocs.io/en/latest/) |
| ddu | 18.0.0.4 | [https://www.wagnardsoft.com/](https://www.wagnardsoft.com/) |
| deadlock | 1.4 | [https://codedead.com/](https://codedead.com/) |
| debugviewpp | 1.8.0.34 | [https://github.com/CobaltFusion/DebugViewPP](https://github.com/CobaltFusion/DebugViewPP) |
| defraggler | 2.22.995 | [https://www.ccleaner.com/defraggler](https://www.ccleaner.com/defraggler) |
| deluge | 1.3.15 | [http://deluge-torrent.org/](http://deluge-torrent.org/) |
| deno | 0.2.2 | [https://github.com/denoland/deno](https://github.com/denoland/deno) |
| dep | 0.5.0 | [https://github.com/golang/dep](https://github.com/golang/dep) |
| dependencies | 1.9 | [https://github.com/lucasg/Dependencies](https://github.com/lucasg/Dependencies) |
| depends | 2.2 | [http://www.dependencywalker.com/](http://www.dependencywalker.com/) |
| devd | 0.8 | [https://corte.si/posts/devd/intro/index.html](https://corte.si/posts/devd/intro/index.html) |
| devdocs | 0.6.9 | [https://github.com/egoist/devdocs-desktop](https://github.com/egoist/devdocs-desktop) |
| devrantron | 1.5.4 | [https://github.com/tahnik/devRantron](https://github.com/tahnik/devRantron) |
| dhcp-server | 2.5.2 | [http://www.dhcpserver.de](http://www.dhcpserver.de) |
| diff-pdf | 2012-02-28 | [http://vslavik.github.io/diff-pdf/](http://vslavik.github.io/diff-pdf/) |
| diffpdf | 2.1.3 | [http://soft.rubypdf.com/software/diffpdf](http://soft.rubypdf.com/software/diffpdf) |
| diffutils | 3.5 | [http://www.msys2.org](http://www.msys2.org) |
| dig | 9.13.4 | [https://www.isc.org/](https://www.isc.org/) |
| digdag | 0.9.31 | [https://www.digdag.io/](https://www.digdag.io/) |
| dirhash | 1.7.1 | [https://idrassi.github.io/DirHash](https://idrassi.github.io/DirHash) |
| discord-canary | 0.0.224 | [https://discordapp.com/](https://discordapp.com/) |
| discord-ptb | 0.0.43 | [https://discordapp.com/](https://discordapp.com/) |
| discord | 0.0.301 | [https://discordapp.com/](https://discordapp.com/) |
| dismplusplus | 10.1.1000.80 | [https://www.chuyu.me](https://www.chuyu.me) |
| ditto | 3.21.258.0 | [http://ditto-cp.sourceforge.net/](http://ditto-cp.sourceforge.net/) |
| dnsjumper | 2.1 | [https://www.sordum.org/dns-jumper/](https://www.sordum.org/dns-jumper/) |
| dnspy | 5.0.0 | [https://github.com/0xd4d/dnSpy](https://github.com/0xd4d/dnSpy) |
| docker-compose | 1.23.2 | [https://github.com/docker/compose](https://github.com/docker/compose) |
| docker-machine | 0.16.0 | [https://github.com/docker/machine](https://github.com/docker/machine) |
| docker-nightly | nightly | [https://master.dockerproject.org](https://master.dockerproject.org) |
| docker | 18.09.0 | [https://docker.com](https://docker.com) |
| dont-sleep | 4.91 | [https://www.softwareok.com/?Download=DontSleep](https://www.softwareok.com/?Download=DontSleep) |
| dopamine | 1.5.14 | [https://www.digimezzo.com/software/dopamine/](https://www.digimezzo.com/software/dopamine/) |
| dos2unix | 7.4.0 | [http://dos2unix.sourceforge.net/](http://dos2unix.sourceforge.net/) |
| dosbox | 0.74-2 | [https://www.dosbox.com/](https://www.dosbox.com/) |
| dotnet-sdk | 2.2.100 | [https://www.microsoft.com/net/](https://www.microsoft.com/net/) |
| dotnet | 1.1.1 | [https://www.microsoft.com/net/core#windows](https://www.microsoft.com/net/core#windows) |
| doublecmd | 0.8.4 | [https://doublecmd.sourceforge.io/](https://doublecmd.sourceforge.io/) |
| doxygen | 1.8.14 | [http://www.doxygen.nl/](http://www.doxygen.nl/) |
| draft | 0.16.0 | [https://github.com/Azure/draft](https://github.com/Azure/draft) |
| drone | 1.0.4 | [https://drone.io/](https://drone.io/) |
| ds4windows | 1.5.18 | [https://ryochan7.github.io/ds4windows-site/](https://ryochan7.github.io/ds4windows-site/) |
| duplicacy | 2.1.2 | [https://duplicacy.com/](https://duplicacy.com/) |
| eagleget-portable | 2.0.4.80 | [http://www.eagleget.com/](http://www.eagleget.com/) |
| easyrsa | 3.0.5 | [https://openvpn.net/easyrsa.html](https://openvpn.net/easyrsa.html) |
| easyserviceoptimizer | 1.2 | [https://www.sordum.org/files/easy-service-optimizer/](https://www.sordum.org/files/easy-service-optimizer/) |
| ec2-api-tools | 1.7.3.0 | [https://aws.amazon.com/developertools/351](https://aws.amazon.com/developertools/351) |
| echoargs | 3.2 | [https://pscx.codeplex.com/](https://pscx.codeplex.com/) |
| eclipse-android | 4.6.3 | [https://www.eclipse.org](https://www.eclipse.org) |
| eclipse-automotive | 4.5.2 | [https://www.eclipse.org](https://www.eclipse.org) |
| eclipse-committers | 2018-09 | [https://www.eclipse.org](https://www.eclipse.org) |
| eclipse-cpp | 2018-09 | [https://www.eclipse.org](https://www.eclipse.org) |
| eclipse-dsl | 2018-09 | [https://www.eclipse.org](https://www.eclipse.org) |
| eclipse-java | 2018-09 | [https://www.eclipse.org](https://www.eclipse.org) |
| eclipse-javascript | 2018-09 | [https://www.eclipse.org](https://www.eclipse.org) |
| eclipse-jee | 2018-09 | [https://www.eclipse.org](https://www.eclipse.org) |
| eclipse-mat | 1.8.1.20180910 | [https://www.eclipse.org/mat/](https://www.eclipse.org/mat/) |
| eclipse-modeling | 2018-09 | [https://www.eclipse.org](https://www.eclipse.org) |
| eclipse-parallel | 2018-09 | [https://www.eclipse.org](https://www.eclipse.org) |
| eclipse-php | 2018-09 | [https://www.eclipse.org](https://www.eclipse.org) |
| eclipse-platform | 4.9-201809060745 | [https://www.eclipse.org](https://www.eclipse.org) |
| eclipse-rcp | 2018-09 | [https://www.eclipse.org](https://www.eclipse.org) |
| eclipse-reporting | 2018-09 | [https://www.eclipse.org](https://www.eclipse.org) |
| eclipse-scout | 2018-09 | [https://www.eclipse.org](https://www.eclipse.org) |
| eclipse-sdk | 4.9-201809060745 | [https://www.eclipse.org](https://www.eclipse.org) |
| eclipse-testing | 2018-09 | [https://www.eclipse.org](https://www.eclipse.org) |
| edex-ui | 1.1.2 | [https://github.com/GitSquared/edex-ui](https://github.com/GitSquared/edex-ui) |
| edgedriver | 6.17134 | [https://developer.microsoft.com/en-us/microsoft-edge/tools/webdriver/#downloads](https://developer.microsoft.com/en-us/microsoft-edge/tools/webdriver/#downloads) |
| editorconfig | 0.12.1 | [http://editorconfig.org/](http://editorconfig.org/) |
| elasticsearch | 6.5.3 | [https://www.elastic.co/products/elasticsearch](https://www.elastic.co/products/elasticsearch) |
| elixir | 1.7.4 | [https://elixir-lang.org/](https://elixir-lang.org/) |
| elm | 0.19.0 | [http://elm-lang.org](http://elm-lang.org) |
| emacs | 26.1 | [https://www.gnu.org/software/emacs/](https://www.gnu.org/software/emacs/) |
| enpass | 5.6.10 | [https://www.enpass.io/](https://www.enpass.io/) |
| enso | 0.4.2 | [https://github.com/GChristensen/enso-portable](https://github.com/GChristensen/enso-portable) |
| erlang | 21.2 | [https://www.erlang.org](https://www.erlang.org) |
| etcher-cli | 1.4.8 | [https://etcher.io/cli](https://etcher.io/cli) |
| etcher | 1.4.8 | [https://etcher.io/](https://etcher.io/) |
| etlas | 1.5.0.0 | [https://github.com/typelead/etlas](https://github.com/typelead/etlas) |
| eventstore | 4.1.1-hotfix1 | [https://eventstore.org/](https://eventstore.org/) |
| everything | 1.4.1.895 | [https://www.voidtools.com/](https://www.voidtools.com/) |
| executor | 0.99.27b | [http://executor.dk/](http://executor.dk/) |
| exercism-cli | 3.0.11 | [http://exercism.io/](http://exercism.io/) |
| exercism | 3.0.11 | [https://github.com/exercism/cli](https://github.com/exercism/cli) |
| exiftool | 11.21 | [https://sno.phy.queensu.ca/~phil/exiftool/index.html](https://sno.phy.queensu.ca/~phil/exiftool/index.html) |
| faas-cli | 0.8.1 | [https://www.openfaas.com/](https://www.openfaas.com/) |
| falcon-sql-client | 4.0.0 | [https://plot.ly/free-sql-client-download](https://plot.ly/free-sql-client-download) |
| far | 30b5300 | [https://farmanager.com/](https://farmanager.com/) |
| fastcopy | 3.61 | [https://fastcopy.jp/en/](https://fastcopy.jp/en/) |
| fastglacier | 3.9.1 | [https://fastglacier.com](https://fastglacier.com) |
| fciv | 2.05 | [https://support.microsoft.com/en-us/kb/841290](https://support.microsoft.com/en-us/kb/841290) |
| fd | 7.2.0 | [https://github.com/sharkdp/fd](https://github.com/sharkdp/fd) |
| ffmpeg-nightly | 20181212-0e833f6 | [https://ffmpeg.zeranoe.com/builds/](https://ffmpeg.zeranoe.com/builds/) |
| ffmpeg | 4.1 | [https://ffmpeg.zeranoe.com/builds/](https://ffmpeg.zeranoe.com/builds/) |
| fiddler | 5.0.20182.28034 | [https://www.telerik.com/fiddler](https://www.telerik.com/fiddler) |
| figlet | 1.0-go | [https://github.com/lukesampson/figlet](https://github.com/lukesampson/figlet) |
| file | 5.03 | [http://gnuwin32.sourceforge.net/packages/file.htm](http://gnuwin32.sourceforge.net/packages/file.htm) |
| filezilla | 3.39.0 | [https://filezilla-project.org/](https://filezilla-project.org/) |
| find-java | 13 | [https://gist.github.com/se35710/43693e679701387d722206eff1e85f5f](https://gist.github.com/se35710/43693e679701387d722206eff1e85f5f) |
| findutils | 4.4.2 | [http://www.mingw.org/wiki/msys](http://www.mingw.org/wiki/msys) |
| firefox-beta | nightly | [https://www.mozilla.org/en-US/firefox/beta/](https://www.mozilla.org/en-US/firefox/beta/) |
| firefox-developer | nightly | [https://www.mozilla.org/en-US/firefox/developer/](https://www.mozilla.org/en-US/firefox/developer/) |
| firefox-esr | 60.4.0 | [https://www.mozilla.org/en-US/firefox/organizations/](https://www.mozilla.org/en-US/firefox/organizations/) |
| firefox-nightly | nightly | [https://www.mozilla.org/en-US/firefox/nightly/](https://www.mozilla.org/en-US/firefox/nightly/) |
| firefox | 64.0 | [https://www.mozilla.org/en-US/firefox/new/](https://www.mozilla.org/en-US/firefox/new/) |
| firewallappblocker | 1.6 | [https://www.sordum.org/files/firewall-app-blocker/](https://www.sordum.org/files/firewall-app-blocker/) |
| flatc | 1.10.0 | [https://google.github.io/flatbuffers/index.html](https://google.github.io/flatbuffers/index.html) |
| flow | 0.88.0 | [https://flowtype.org/](https://flowtype.org/) |
| flutter | 0.10.2 | [https://flutter.io/](https://flutter.io/) |
| flux | 4.84 | [https://justgetflux.com/](https://justgetflux.com/) |
| flyway | 5.2.4 | [https://flywaydb.org/](https://flywaydb.org/) |
| fmedia | 1.3 | [http://fmedia.firmdev.com/](http://fmedia.firmdev.com/) |
| fnproject | 0.5.35 | [https://fnproject.io/](https://fnproject.io/) |
| fnr | 1.8.1 | [https://github.com/zzzprojects/findandreplace](https://github.com/zzzprojects/findandreplace) |
| fontforge | 20170731-r2 | [https://fontforge.github.io](https://fontforge.github.io) |
| foobar2000-encoders | 2018-10-19 | [https://www.foobar2000.org/encoderpack](https://www.foobar2000.org/encoderpack) |
| foobar2000 | 1.4.1 | [https://www.foobar2000.org/](https://www.foobar2000.org/) |
| force | 0.25.0 | [https://force-cli.herokuapp.com/](https://force-cli.herokuapp.com/) |
| forego | 20180217041714 | [https://github.com/ddollar/forego](https://github.com/ddollar/forego) |
| forge | 2.2.0 | [http://forge.run](http://forge.run) |
| format-factory | 4.5.0.0 | [http://www.pcfreetime.com/formatfactory/index.php](http://www.pcfreetime.com/formatfactory/index.php) |
| fossil | 2.7 | [https://www.fossil-scm.org/](https://www.fossil-scm.org/) |
| foxe | 2.4.2 | [http://www.firstobject.com/dn_editor.htm](http://www.firstobject.com/dn_editor.htm) |
| foxit-reader | 9.3.0.10826 | [https://www.foxitsoftware.com/](https://www.foxitsoftware.com/) |
| franz | 5.0.0-beta.19 | [http://meetfranz.com](http://meetfranz.com) |
| freac | 1.0.32 | [https://www.freac.org](https://www.freac.org) |
| freeclipboardviewer | 3.0 | [http://www.freeclipboardviewer.com/](http://www.freeclipboardviewer.com/) |
| freecommander | 2018 | [https://freecommander.com](https://freecommander.com) |
| freemind | 1.0.1 | [http://freemind.sourceforge.net/wiki/index.php/Main_Page](http://freemind.sourceforge.net/wiki/index.php/Main_Page) |
| fscapture | 5.3 | [http://www.faststone.org/FSCaptureDetail.htm](http://www.faststone.org/FSCaptureDetail.htm) |
| fsviewer | 6.7 | [http://www.faststone.org/FSViewerDetail.htm](http://www.faststone.org/FSViewerDetail.htm) |
| fzf | 0.17.5 | [https://github.com/junegunn/fzf](https://github.com/junegunn/fzf) |
| gawk | 3.1.7 | [http://www.mingw.org/wiki/MSYS](http://www.mingw.org/wiki/MSYS) |
| gcc-arm-none-eabi | 7-2018-q2-update | [https://developer.arm.com/open-source/gnu-toolchain/gnu-rm](https://developer.arm.com/open-source/gnu-toolchain/gnu-rm) |
| gcc | 8.1.0 | [https://mingw-w64.org](https://mingw-w64.org) |
| gcloud | 228.0.0 | [https://cloud.google.com/sdk/](https://cloud.google.com/sdk/) |
| gdb | 7.9.1 | [http://tdm-gcc.tdragon.net/](http://tdm-gcc.tdragon.net/) |
| geany | 1.33 | [https://www.geany.org/](https://www.geany.org/) |
| geckodriver | 0.23.0 | [https://github.com/mozilla/geckodriver](https://github.com/mozilla/geckodriver) |
| geekuninstaller | 1.4.5.134 | [https://geekuninstaller.com/](https://geekuninstaller.com/) |
| genact | 0.6.0 | [https://github.com/svenstaro/genact/](https://github.com/svenstaro/genact/) |
| ghostscript | 9.26 | [https://www.ghostscript.com](https://www.ghostscript.com) |
| ghostwriter | 1.7.1 | [https://wereturtle.github.io/ghostwriter/](https://wereturtle.github.io/ghostwriter/) |
| ghq | 0.8.0 | [https://github.com/motemen/ghq](https://github.com/motemen/ghq) |
| gibo | 2.1.0 | [https://github.com/simonwhitaker/gibo](https://github.com/simonwhitaker/gibo) |
| gifcam | 5.5 | [http://blog.bahraniapps.com/gifcam/](http://blog.bahraniapps.com/gifcam/) |
| gifsicle | 1.89 | [http://www.lcdf.org/gifsicle/](http://www.lcdf.org/gifsicle/) |
| gimp | 2.10.8 | [https://www.gimp.org/](https://www.gimp.org/) |
| git-annex | 7.20181211 | [http://git-annex.branchable.com/](http://git-annex.branchable.com/) |
| git-crypt | 0.6.0-701fb8e | [https://www.agwa.name/projects/git-crypt/](https://www.agwa.name/projects/git-crypt/) |
| git-istage | 0.2.61 | [https://github.com/terrajobst/git-istage](https://github.com/terrajobst/git-istage) |
| git-lfs | 2.6.1 | [https://git-lfs.github.com/](https://git-lfs.github.com/) |
| git-sizer | 1.3.0 | [https://github.com/github/git-sizer](https://github.com/github/git-sizer) |
| git-town | 7.2.0 | [http://www.git-town.com/](http://www.git-town.com/) |
| git-up | 1.6.0 | [https://github.com/msiemens/PyGitUp](https://github.com/msiemens/PyGitUp) |
| git-with-openssh | 2.20.0.windows.1 | [https://git-for-windows.github.io/](https://git-for-windows.github.io/) |
| git | 2.20.0.windows.1 | [https://git-for-windows.github.io/](https://git-for-windows.github.io/) |
| git19 | 1.9.5-preview20150319 | [https://git-for-windows.github.io/](https://git-for-windows.github.io/) |
| gitea | 1.6.1 | [https://gitea.io/](https://gitea.io/) |
| gitextensions | 2.51.05 | [https://gitextensions.github.io/](https://gitextensions.github.io/) |
| github | 1.5.0 | [https://desktop.github.com/](https://desktop.github.com/) |
| gitignore | 0.2018.08.04 | [https://github.com/lukesampson/psutils](https://github.com/lukesampson/psutils) |
| gitkraken | 4.1.1 | [https://www.gitkraken.com/](https://www.gitkraken.com/) |
| gitlab-runner | 11.5.1 | [https://docs.gitlab.com/runner/](https://docs.gitlab.com/runner/) |
| gitversion | 4.0.0 | [https://gitversion.readthedocs.io/](https://gitversion.readthedocs.io/) |
| glide | 0.13.2 | [https://glide.sh/](https://glide.sh/) |
| glogg | 1.1.4 | [https://glogg.bonnefon.org/](https://glogg.bonnefon.org/) |
| glslang-nightly | nightly | [https://www.khronos.org/opengles/sdk/tools/Reference-Compiler/](https://www.khronos.org/opengles/sdk/tools/Reference-Compiler/) |
| glslang | 7.10.2984 | [https://www.khronos.org/opengles/sdk/tools/Reference-Compiler/](https://www.khronos.org/opengles/sdk/tools/Reference-Compiler/) |
| gnirehtet | 2.3 | [https://github.com/Genymobile/gnirehtet](https://github.com/Genymobile/gnirehtet) |
| gnucash | 3.2 | [https://www.gnucash.org/](https://www.gnucash.org/) |
| gnupg | 2.2.11 | [https://www.gnupg.org/](https://www.gnupg.org/) |
| gnupg1 | 1.4.23 | [https://www.gnupg.org/](https://www.gnupg.org/) |
| go-ipfs | 0.4.18 | [https://ipfs.io/](https://ipfs.io/) |
| go | 1.11.2 | [https://golang.org](https://golang.org) |
| godot-mono | 3.0.6 | [https://godotengine.org/](https://godotengine.org/) |
| godot | 3.0.6 | [https://godotengine.org/](https://godotengine.org/) |
| gof | 0.0.1 | [https://github.com/mattn/gof](https://github.com/mattn/gof) |
| gogs | 0.11.79 | [https://gogs.io/](https://gogs.io/) |
| goldendict | 1.5.0-RC2-311-g15062f7 | [https://sourceforge.net/projects/goldendict/](https://sourceforge.net/projects/goldendict/) |
| google-java-format | 1.6 | [https://github.com/google/google-java-format](https://github.com/google/google-java-format) |
| gopass | 1.8.3 | [https://www.gopass.pw/](https://www.gopass.pw/) |
| gource | 0.47 | [http://gource.io/](http://gource.io/) |
| gow | 0.8.0 | [https://github.com/bmatzelle/gow](https://github.com/bmatzelle/gow) |
| gpg | 2.2.11 | [https://www.gnupg.org/](https://www.gnupg.org/) |
| gpg4win | 3.1.5 | [https://www.gpg4win.org](https://www.gpg4win.org) |
| gpu-z | 2.16.0 | [https://www.techpowerup.com/gpuz/](https://www.techpowerup.com/gpuz/) |
| gradle-bin | 5.0 | [https://gradle.org](https://gradle.org) |
| gradle | 5.0 | [https://gradle.org](https://gradle.org) |
| grafana | 5.4.1 | [https://grafana.com/](https://grafana.com/) |
| grails | 3.3.9 | [https://grails.org/](https://grails.org/) |
| graphicsgale | 2.08.19 | [https://graphicsgale.com/us/](https://graphicsgale.com/us/) |
| graphicsmagick-q16 | 1.3.31 | [http://www.graphicsmagick.org/](http://www.graphicsmagick.org/) |
| graphicsmagick-q8 | 1.3.31 | [http://www.graphicsmagick.org/](http://www.graphicsmagick.org/) |
| graphviz | 2.38 | [https://www.graphviz.org/](https://www.graphviz.org/) |
| greenshot | 1.2.10.6 | [https://getgreenshot.org](https://getgreenshot.org) |
| grep | 2.5.4 | [http://gnuwin32.sourceforge.net/packages/grep.htm](http://gnuwin32.sourceforge.net/packages/grep.htm) |
| groovy | 2.5.4 | [http://www.groovy-lang.org/](http://www.groovy-lang.org/) |
| groovyserv | 1.2.0 | [https://kobo.github.io/groovyserv/](https://kobo.github.io/groovyserv/) |
| guetzli | 1.0.1 | [https://github.com/google/guetzli](https://github.com/google/guetzli) |
| gzip | 1.3.12 | [http://www.mingw.org/wiki/msys](http://www.mingw.org/wiki/msys) |
| hack-font | 1.6.0 | [https://sourcefoundry.org/hack/](https://sourcefoundry.org/hack/) |
| hadoop-winutils | 2.8.1 | [https://github.com/steveloughran/winutils](https://github.com/steveloughran/winutils) |
| hain | 0.6.6 | [http://hainproject.github.io/hain/](http://hainproject.github.io/hain/) |
| HamMultiPlayer | 0.116.37905.792 | [http://hammultiplayer.org](http://hammultiplayer.org) |
| handbrake-cli | 1.1.2 | [https://handbrake.fr/](https://handbrake.fr/) |
| handbrake | 1.1.2 | [https://handbrake.fr/](https://handbrake.fr/) |
| harmony | 0.9.1 | [https://getharmony.xyz/](https://getharmony.xyz/) |
| hashcat | 5.1.0 | [https://hashcat.net/hashcat/](https://hashcat.net/hashcat/) |
| haskell | 8.4.3 | [https://www.haskell.org](https://www.haskell.org) |
| haskellx | 7.8.3 | [https://www.haskell.org](https://www.haskell.org) |
| haxe | 3.4.7 | [https://haxe.org/](https://haxe.org/) |
| heidisql | 9.5 | [https://www.heidisql.com/](https://www.heidisql.com/) |
| helm | 2.12.0 | [https://helm.sh/](https://helm.sh/) |
| helmfile | 0.40.3 | [https://github.com/roboll/helmfile/](https://github.com/roboll/helmfile/) |
| heroku-cli | nightly | []() |
| hexchat | 2.14.2 | [https://hexchat.github.io](https://hexchat.github.io) |
| highlight | 3.47 | [http://www.andre-simon.de/doku/highlight/en/highlight.php](http://www.andre-simon.de/doku/highlight/en/highlight.php) |
| honeyview | 5.31 | [https://www.bandisoft.com/honeyview/](https://www.bandisoft.com/honeyview/) |
| hostsman | 4.7.105 | [http://www.abelhadigital.com/hostsman](http://www.abelhadigital.com/hostsman) |
| httrack | 3.49.2 | [https://www.httrack.com/](https://www.httrack.com/) |
| hub | 2.6.1 | [https://hub.github.com/](https://hub.github.com/) |
| hugo | 0.52 | [https://gohugo.io](https://gohugo.io) |
| hwinfo | 5.92-3580 | [https://www.hwinfo.com/](https://www.hwinfo.com/) |
| hwmonitor | 1.38 | [https://www.cpuid.com/softwares/hwmonitor.html](https://www.cpuid.com/softwares/hwmonitor.html) |
| hxd | 2.1.0.0 | [https://mh-nexus.de/en/hxd/](https://mh-nexus.de/en/hxd/) |
| hygen | 1.6.4 | [https://www.hygen.io/](https://www.hygen.io/) |
| hyper | 2.0.0 | [https://hyper.is](https://hyper.is) |
| hyperfine | 1.4.0 | [https://github.com/sharkdp/hyperfine](https://github.com/sharkdp/hyperfine) |
| ibmcloud-cli | 0.12.1 | [https://github.com/IBM-Bluemix/bluemix-cli-release](https://github.com/IBM-Bluemix/bluemix-cli-release) |
| iconv | 1.14-3 | [http://www.mingw.org/](http://www.mingw.org/) |
| idea-eap | 183.4139.22 | [https://www.jetbrains.com/idea/](https://www.jetbrains.com/idea/) |
| idea-ultimate-eap | 183.4139.22 | [https://www.jetbrains.com/idea/](https://www.jetbrains.com/idea/) |
| idea-ultimate | 2018.3.1 | [https://www.jetbrains.com/idea/](https://www.jetbrains.com/idea/) |
| idea | 2018.3.1 | [https://www.jetbrains.com/idea/](https://www.jetbrains.com/idea/) |
| idris | 1.3.1 | [https://www.idris-lang.org/](https://www.idris-lang.org/) |
| ie11webdriver | 3.14.0 | [http://www.seleniumhq.org/](http://www.seleniumhq.org/) |
| ilspy | 3.2.0.3856 | [http://ilspy.net/](http://ilspy.net/) |
| imageglass | 5.5.7.26 | [http://www.imageglass.org/](http://www.imageglass.org/) |
| imagemagick | 7.0.8-16 | [https://www.imagemagick.org/script/index.php](https://www.imagemagick.org/script/index.php) |
| imgburn | 2.5.8.0 | [http://www.imgburn.com/](http://www.imgburn.com/) |
| inadyn-mt | 02.28.10 | [https://sourceforge.net/projects/inadyn-mt/files/inadyn-mt/](https://sourceforge.net/projects/inadyn-mt/files/inadyn-mt/) |
| inboxer | 1.2.1 | [https://denysdovhan.com/inboxer/](https://denysdovhan.com/inboxer/) |
| influxdb | 1.7.1 | [https://www.influxdata.com/](https://www.influxdata.com/) |
| inkscape | 0.92.3 | [https://inkscape.org/](https://inkscape.org/) |
| inkscape32bit | 0.92.3 | [https://inkscape.org/](https://inkscape.org/) |
| innoextract | 1.7 | [http://constexpr.org/innoextract/](http://constexpr.org/innoextract/) |
| innounp | 0.47 | [http://innounp.sourceforge.net](http://innounp.sourceforge.net) |
| insect | 5.0.0 | [https://github.com/sharkdp/insect](https://github.com/sharkdp/insect) |
| insomnia | 6.2.3 | [https://insomnia.rest](https://insomnia.rest) |
| invoke-build | 5.4.2 | [https://github.com/nightroman/Invoke-Build](https://github.com/nightroman/Invoke-Build) |
| iographica | 1.0.1 | [http://www.iographica.com/](http://www.iographica.com/) |
| ios-webkit-debug-proxy | 1.8.3 | [https://github.com/google/ios-webkit-debug-proxy](https://github.com/google/ios-webkit-debug-proxy) |
| iperf3 | 3.1.3 | [https://iperf.fr/](https://iperf.fr/) |
| ipfilter-updater | 3.0.0 | [https://www.sadrobot.co.nz/ipfilter/](https://www.sadrobot.co.nz/ipfilter/) |
| ipscan | 3.5.3 | [http://angryip.org/](http://angryip.org/) |
| irfanview | 4.51 | [https://www.irfanview.com/](https://www.irfanview.com/) |
| jameica | 2.8.2 | [https://www.willuhn.de/products/jameica/](https://www.willuhn.de/products/jameica/) |
| jd-cmd | 0.9.2 | [https://github.com/kwart/jd-cmd](https://github.com/kwart/jd-cmd) |
| jd-gui | 1.4.0 | [http://jd.benow.ca/](http://jd.benow.ca/) |
| jdownloader | nightly | [http://jdownloader.org/](http://jdownloader.org/) |
| jetbrains-toolbox | 1.12.4481 | [https://jetbrains.com/](https://jetbrains.com/) |
| jfrog | 1.22.1 | [https://jfrog.com/getcli/](https://jfrog.com/getcli/) |
| jhead | 3.00 | [http://www.sentex.net/~mwandel/jhead/](http://www.sentex.net/~mwandel/jhead/) |
| jigsaw | 2.2.6 | [https://www.w3.org/Jigsaw](https://www.w3.org/Jigsaw) |
| jira | 1.0.20 | [https://github.com/Netflix-Skunkworks/go-jira](https://github.com/Netflix-Skunkworks/go-jira) |
| jitsi-meet-electron | 1.1.1 | [https://github.com/jitsi/jitsi-meet-electron](https://github.com/jitsi/jitsi-meet-electron) |
| jkrypto | 4.4 | [http://lpb.canb.auug.org.au/adfa/src/jkrypto/index.html](http://lpb.canb.auug.org.au/adfa/src/jkrypto/index.html) |
| joe | 4.6 | [https://joe-editor.sourceforge.io/](https://joe-editor.sourceforge.io/) |
| joplin | 1.0.117 | [https://joplin.cozic.net/](https://joplin.cozic.net/) |
| jpegview | 1.0.37 | [https://downloads.sourceforge.net/project/jpegview/](https://downloads.sourceforge.net/project/jpegview/) |
| jq | 1.6 | [https://stedolan.github.io/jq/](https://stedolan.github.io/jq/) |
| jruby | 9.2.5.0 | [https://www.jruby.org/](https://www.jruby.org/) |
| julia | 1.0.2 | [https://julialang.org](https://julialang.org) |
| just | 0.3.13 | [https://github.com/casey/just](https://github.com/casey/just) |
| kakaotalk | 2.7.0.1858 | [https://www.kakao.com/talk](https://www.kakao.com/talk) |
| kdenlive | 18.08.2 | [https://kdenlive.org/](https://kdenlive.org/) |
| kdiff3 | 0.9.98 | [http://kdiff3.sourceforge.net/](http://kdiff3.sourceforge.net/) |
| keepass | 2.40 | [https://keepass.info/](https://keepass.info/) |
| keepassxc | 2.3.4 | [https://keepassxc.org/](https://keepassxc.org/) |
| keeweb | 1.6.3 | [https://keeweb.info/](https://keeweb.info/) |
| keypirinha | 2.23 | [http://keypirinha.com](http://keypirinha.com) |
| keystore-explorer | 5.4.1 | [https://keystore-explorer.org/](https://keystore-explorer.org/) |
| kibana | 6.5.3 | [https://www.elastic.co/products/kibana](https://www.elastic.co/products/kibana) |
| kicad | 5.0.2_1 | [http://kicad-pcb.org/](http://kicad-pcb.org/) |
| kid3 | 3.6.2 | [https://kid3.sourceforge.io](https://kid3.sourceforge.io) |
| kindlegen | 2.9 | [https://www.amazon.com/gp/feature.html?docId=1000765211](https://www.amazon.com/gp/feature.html?docId=1000765211) |
| kitematic | 0.17.6 | [https://github.com/docker/kitematic](https://github.com/docker/kitematic) |
| kitty | 0.70.0.7 | [http://kitty.9bis.net](http://kitty.9bis.net) |
| knime | 3.7.0 | [https://www.knime.com/](https://www.knime.com/) |
| kompose | 1.17.0 | [http://kompose.io](http://kompose.io) |
| kotlin-native | 0.9.3 | [https://kotlinlang.org/](https://kotlinlang.org/) |
| kotlin | 1.3.11 | [https://kotlinlang.org/](https://kotlinlang.org/) |
| krita | 4.1.5 | [https://krita.org/](https://krita.org/) |
| ktlint | 0.29.0 | [https://github.com/shyiko/ktlint](https://github.com/shyiko/ktlint) |
| kubectl | 1.13.0 | [https://kubernetes.io/docs/user-guide/kubectl-overview/](https://kubernetes.io/docs/user-guide/kubectl-overview/) |
| lame | 3.100 | [https://lame.sourceforge.net/](https://lame.sourceforge.net/) |
| latex | 2.9.6753 | [https://miktex.org](https://miktex.org) |
| launchy | 2.9.57 | [https://openningia.github.io/Launchy](https://openningia.github.io/Launchy) |
| lazygit | 0.5 | [https://github.com/jesseduffield/lazygit](https://github.com/jesseduffield/lazygit) |
| lcow | v4.14.35-v0.3.9 | [https://github.com/linuxkit/lcow](https://github.com/linuxkit/lcow) |
| ldap-admin | 1.8.3 | [http://ldapadmin.org/](http://ldapadmin.org/) |
| ldc | 1.12.0 | [https://dlang.org/](https://dlang.org/) |
| leet | 2014.8.29 | [https://github.com/vidarkongsli/posh1337](https://github.com/vidarkongsli/posh1337) |
| leiningen | 2.8.2 | [https://github.com/technomancy/leiningen](https://github.com/technomancy/leiningen) |
| less | 530 | [http://www.greenwoodsoftware.com/less/](http://www.greenwoodsoftware.com/less/) |
| lessmsi | 1.6.3 | [https://github.com/activescott/lessmsi/](https://github.com/activescott/lessmsi/) |
| lf | r8 | [https://godoc.org/github.com/gokcehan/lf](https://godoc.org/github.com/gokcehan/lf) |
| libreoffice-fresh | 6.1.3.2 | [https://libreoffice.org/](https://libreoffice.org/) |
| libsndfile | 1.0.28 | [http://www.mega-nerd.com/libsndfile/](http://www.mega-nerd.com/libsndfile/) |
| libwebp | 1.0.0 | [https://developers.google.com/speed/webp/](https://developers.google.com/speed/webp/) |
| licecap | 1.26 | [https://www.cockos.com/licecap/](https://www.cockos.com/licecap/) |
| lightbulb | 1.6.4.1 | [https://github.com/Tyrrrz/LightBulb](https://github.com/Tyrrrz/LightBulb) |
| lightshot | nightly | [https://prnt.sc](https://prnt.sc) |
| lighttable | 0.8.1 | [http://www.lighttable.com/](http://www.lighttable.com/) |
| lighttpd | 1.4.49-1 | [http://lighttpd.dtech.hu/](http://lighttpd.dtech.hu/) |
| lili | 2.9.4 | [https://www.linuxliveusb.com](https://www.linuxliveusb.com) |
| lilypond | 2.18.2 | [http://lilypond.org](http://lilypond.org) |
| linqpad | nightly | [https://www.linqpad.net](https://www.linqpad.net) |
| linqpadless | 1.1.0 | [https://github.com/linqpadless/LinqPadless](https://github.com/linqpadless/LinqPadless) |
| listenmoeclient | 2.0.0 | [https://github.com/LISTEN-moe/windows-app](https://github.com/LISTEN-moe/windows-app) |
| llvm | 7.0.0 | [https://www.llvm.org/](https://www.llvm.org/) |
| lmms | 1.1.3 | [https://lmms.io/](https://lmms.io/) |
| ln | 0.2018.08.04 | [https://github.com/lukesampson/psutils](https://github.com/lukesampson/psutils) |
| lockhunter | 3.2.3 | [https://lockhunter.com/index.htm](https://lockhunter.com/index.htm) |
| logexpert | 1.6.13 | [https://github.com/zarunbal/LogExpert](https://github.com/zarunbal/LogExpert) |
| logstash | 5.6.1 | [https://www.elastic.co/products/logstash](https://www.elastic.co/products/logstash) |
| losslesscut | 1.14.0 | [https://github.com/mifi/lossless-cut](https://github.com/mifi/lossless-cut) |
| love | 11.2 | [https://love2d.org/](https://love2d.org/) |
| lua | 5.1.5-52 | [https://github.com/rjpcomputing/luaforwindows](https://github.com/rjpcomputing/luaforwindows) |
| lunacy | 3.12 | [https://icons8.com/lunacy](https://icons8.com/lunacy) |
| lxrunoffline | 3.3.2 | [https://github.com/DDoSolitary/LxRunOffline](https://github.com/DDoSolitary/LxRunOffline) |
| lynx | 2.8.9rel.1 | [http://invisible-island.net/lynx/lynx.html](http://invisible-island.net/lynx/lynx.html) |
| lzip | 1.20 | [https://www.nongnu.org/lzip/lzip.html](https://www.nongnu.org/lzip/lzip.html) |
| madvr | 0.92.17 | [http://madvr.com/](http://madvr.com/) |
| mailsend | 1.19 | [https://github.com/muquit/mailsend](https://github.com/muquit/mailsend) |
| make | 4.2 | [https://www.gnu.org/software/make/](https://www.gnu.org/software/make/) |
| makemkv | 1.14.2 | [https://www.makemkv.com/](https://www.makemkv.com/) |
| mancy | 3.2.0 | [http://mancy-re.pl/](http://mancy-re.pl/) |
| mariadb | 10.3.11 | [https://mariadb.org](https://mariadb.org) |
| maven | 3.6.0 | [https://maven.apache.org/](https://maven.apache.org/) |
| mc | 4.8.19 | [https://midnight-commander.org/](https://midnight-commander.org/) |
| MediaCreationTool | 10.0.17763.1 | [https://www.microsoft.com/en-us/software-download/windows10](https://www.microsoft.com/en-us/software-download/windows10) |
| mediainfo-gui | 18.12 | [https://mediaarea.net/en/MediaInfo](https://mediaarea.net/en/MediaInfo) |
| mediainfo | 18.12 | [https://mediaarea.net/en/MediaInfo](https://mediaarea.net/en/MediaInfo) |
| megasync | 3.7.1.0 | [https://mega.nz/](https://mega.nz/) |
| meld | 3.18.3 | [http://meldmerge.org/](http://meldmerge.org/) |
| mercurial | 4.8.1 | [https://www.mercurial-scm.org/](https://www.mercurial-scm.org/) |
| metastore | 1.1.2-9-gdafa727 | [https://github.com/rasa/metastore](https://github.com/rasa/metastore) |
| micro | 1.4.1 | [https://micro-editor.github.io/](https://micro-editor.github.io/) |
| microsip | 3.19.8 | [https://www.microsip.org](https://www.microsip.org) |
| mill | 0.3.5 | [http://www.lihaoyi.com/mill/](http://www.lihaoyi.com/mill/) |
| mingit-busybox | 2.20.0.windows.1 | [https://git-for-windows.github.io/](https://git-for-windows.github.io/) |
| mingit | 2.20.0.windows.1 | [https://git-for-windows.github.io/](https://git-for-windows.github.io/) |
| miniconda3 | 4.5.11 | [https://conda.io/miniconda.html](https://conda.io/miniconda.html) |
| minikube | 0.31.0 | [https://kubernetes.io/docs/getting-started-guides/minikube/](https://kubernetes.io/docs/getting-started-guides/minikube/) |
| minio-client | 2018-12-05T22-59-07Z | [https://minio.io/](https://minio.io/) |
| minio | 2018-12-06T01-27-43Z | [https://minio.io/](https://minio.io/) |
| minishift | 1.28.0 | [https://www.openshift.org/minishift](https://www.openshift.org/minishift) |
| minisign | 0.8 | [https://jedisct1.github.io/minisign/](https://jedisct1.github.io/minisign/) |
| mitmproxy | 4.0.4 | [https://mitmproxy.org/](https://mitmproxy.org/) |
| mkcert | 1.1.2 | [https://github.com/FiloSottile/mkcert](https://github.com/FiloSottile/mkcert) |
| mkvtoolnix | 29.0.0 | [https://mkvtoolnix.download/](https://mkvtoolnix.download/) |
| mls-software-openssh | 7.9p1-1 | [https://www.mls-software.com/opensshd.html](https://www.mls-software.com/opensshd.html) |
| mobaxterm | 11.0 | [https://mobaxterm.mobatek.net/](https://mobaxterm.mobatek.net/) |
| modd | 0.7 | [https://corte.si/posts/modd/announce/index.html](https://corte.si/posts/modd/announce/index.html) |
| monero | 0.13.0.4 | [https://getmonero.org/](https://getmonero.org/) |
| mongodb-compass-community | 1.16.3 | [https://www.mongodb.com/download-center?jmp=hero#compass](https://www.mongodb.com/download-center?jmp=hero#compass) |
| mongodb | 4.0.4 | [https://www.mongodb.org](https://www.mongodb.org) |
| mono | 5.16.0.220 | [http://www.mono-project.com/](http://www.mono-project.com/) |
| moonscript | 0.5.0 | [https://moonscript.org/](https://moonscript.org/) |
| mousejiggler | 1.7.4 | [https://github.com/cerebrate/mousejiggler](https://github.com/cerebrate/mousejiggler) |
| mozjpeg | 3.3.1 | [https://github.com/mozilla/mozjpeg](https://github.com/mozilla/mozjpeg) |
| mp3tag | 2.91 | [https://www.mp3tag.de/](https://www.mp3tag.de/) |
| mpc-be | 1.5.2 | [https://sourceforge.net/projects/mpcbe/](https://sourceforge.net/projects/mpcbe/) |
| mpc-hc-fork | 1.8.3 | [https://github.com/clsid2/mpc-hc](https://github.com/clsid2/mpc-hc) |
| mpc-hc | 1.7.13 | [https://mpc-hc.org/](https://mpc-hc.org/) |
| mpc-qt | 18.08 | [https://github.com/cmdrkotori/mpc-qt](https://github.com/cmdrkotori/mpc-qt) |
| mplayer | 38117 | [http://mplayerwin.sourceforge.net/](http://mplayerwin.sourceforge.net/) |
| mpv-git | 20181202 | [https://mpv.io/](https://mpv.io/) |
| mpv | 2018-10-02 | [https://mpv.io/](https://mpv.io/) |
| mqtt-spy | 1.0.0 | [https://github.com/eclipse/paho.mqtt-spy](https://github.com/eclipse/paho.mqtt-spy) |
| mremoteng | 1.76.11.40527 | [https://mremoteng.org/](https://mremoteng.org/) |
| msiafterburner | 4.5.0 | [https://www.msi.com/page/afterburner](https://www.msi.com/page/afterburner) |
| msmpi | 9.0.1 | [https://www.microsoft.com/en-us/download/details.aspx?id=56727](https://www.microsoft.com/en-us/download/details.aspx?id=56727) |
| msys | rev13 | []() |
| msys2 | 20180531 | [http://msys2.github.io](http://msys2.github.io) |
| mupdf | 1.14.0 | [https://mupdf.com/](https://mupdf.com/) |
| musescore | 2.3.2 | [https://musescore.org/](https://musescore.org/) |
| musicbee | 3.2.6827 | [https://getmusicbee.com/](https://getmusicbee.com/) |
| mysql-workbench | 8.0.13 | [https://dev.mysql.com/downloads/workbench/](https://dev.mysql.com/downloads/workbench/) |
| mysql | 8.0.13 | [https://dev.mysql.com/downloads/mysql/](https://dev.mysql.com/downloads/mysql/) |
| nano | 2.5.3 | [https://www.nano-editor.org/](https://www.nano-editor.org/) |
| naps2 | 5.8.2 | [https://www.naps2.com/](https://www.naps2.com/) |
| nasm | 2.14 | [http://www.nasm.us](http://www.nasm.us) |
| natural-docs | 2.0.2 | [http://www.naturaldocs.org/](http://www.naturaldocs.org/) |
| ncftpclient | 3.2.6 | [https://www.ncftp.com/](https://www.ncftp.com/) |
| neko | 2.2.0 | [https://nekovm.org/](https://nekovm.org/) |
| neofetch | 5.0.0 | [https://github.com/dylanaraps/neofetch](https://github.com/dylanaraps/neofetch) |
| neovim | 0.3.1 | [https://neovim.io/](https://neovim.io/) |
| netbeans | 9.0 | [https://netbeans.org](https://netbeans.org) |
| netcat | 1.12 | [https://eternallybored.org/misc/netcat/](https://eternallybored.org/misc/netcat/) |
| netlifyctl | 0.4.0 | [https://www.netlify.com/](https://www.netlify.com/) |
| nexusfont | 2.6.2.1870 | [http://www.xiles.net/](http://www.xiles.net/) |
| nginx | 1.15.7 | [https://nginx.org](https://nginx.org) |
| ngrok | 4VmDzA7iaHb | [https://ngrok.com/](https://ngrok.com/) |
| nikto | 2.1.5 | [https://projects.giacomodrago.com/nikto-win/](https://projects.giacomodrago.com/nikto-win/) |
| nim | 0.19.0 | [https://nim-lang.org/](https://nim-lang.org/) |
| nimbleset | 2.2.0.41590 | [http://nimbletext.com/SET/About](http://nimbletext.com/SET/About) |
| nimbletext | 2.9.1.36018 | [http://nimbletext.com/](http://nimbletext.com/) |
| ninja | 1.8.2 | [https://ninja-build.org/](https://ninja-build.org/) |
| nircmd | 2.81 | [https://www.nirsoft.net/utils/nircmd.html](https://www.nirsoft.net/utils/nircmd.html) |
| nirlauncher | 1.20.64 | [https://launcher.nirsoft.net/](https://launcher.nirsoft.net/) |
| nmap | 7.70 | [https://nmap.org](https://nmap.org) |
| node-chakracore | 10.13.0 | [https://github.com/nodejs/node-chakracore](https://github.com/nodejs/node-chakracore) |
| node-compiler | 1.5.0 | [https://github.com/lastmjs/node-compiler](https://github.com/lastmjs/node-compiler) |
| nodejs-lts | 10.14.2 | [https://nodejs.org](https://nodejs.org) |
| nodejs | 11.4.0 | [https://nodejs.org](https://nodejs.org) |
| nomacs | 3.12.1 | [https://nomacs.org](https://nomacs.org) |
| notepad2-mod | 4.2.25.998 | [https://github.com/XhmikosR/notepad2-mod](https://github.com/XhmikosR/notepad2-mod) |
| notepad2 | 4.2.25 | [http://www.flos-freeware.ch/notepad2.html](http://www.flos-freeware.ch/notepad2.html) |
| notepadplusplus-pm | 1.4.12 | [https://bruderste.in/npp/pm/](https://bruderste.in/npp/pm/) |
| notepadplusplus | 7.6 | [https://notepad-plus-plus.org/](https://notepad-plus-plus.org/) |
| now-cli | 12.1.11 | [https://zeit.co/now](https://zeit.co/now) |
| nsis | 3.03 | [http://nsis.sourceforge.net/](http://nsis.sourceforge.net/) |
| nssm | 2.24 | [https://nssm.cc](https://nssm.cc) |
| nteract | 0.12.3 | [https://nteract.io/](https://nteract.io/) |
| nuget-package-explorer | 5.0.116 | [https://github.com/NuGetPackageExplorer/NuGetPackageExplorer](https://github.com/NuGetPackageExplorer/NuGetPackageExplorer) |
| nuget | 4.8.1 | [https://www.nuget.org/](https://www.nuget.org/) |
| nvm | 1.1.7 | [https://github.com/coreybutler/nvm-windows](https://github.com/coreybutler/nvm-windows) |
| nwjs-sdk | 0.35.1 | [https://nwjs.io/](https://nwjs.io/) |
| nwjs | 0.35.1 | [https://nwjs.io/](https://nwjs.io/) |
| obs-studio-small | 21.1.2 | [https://obsproject.com/](https://obsproject.com/) |
| obs-studio | 22.0.2 | [https://obsproject.com/](https://obsproject.com/) |
| ocenaudio | 3.5.4 | [https://www.ocenaudio.com/](https://www.ocenaudio.com/) |
| octave | 4.4.1 | [https://www.gnu.org/software/octave/](https://www.gnu.org/software/octave/) |
| oh-my-posh | 2.0.230 | [https://github.com/JanDeDobbeleer/oh-my-posh](https://github.com/JanDeDobbeleer/oh-my-posh) |
| omnisharp | 1.32.8 | [http://www.omnisharp.net](http://www.omnisharp.net) |
| onefetch | 1.0.0 | [https://github.com/o2sh/onefetch](https://github.com/o2sh/onefetch) |
| oneget | nightly | [https://oneget.org](https://oneget.org) |
| oni | 0.3.6 | [https://www.onivim.io/](https://www.onivim.io/) |
| openhab | 2.3.0 | [https://www.openhab.org/](https://www.openhab.org/) |
| openhardwaremonitor | 0.8.0 | [http://openhardwaremonitor.org/](http://openhardwaremonitor.org/) |
| openliberty | 18.0.0.3 | [https://openliberty.io/](https://openliberty.io/) |
| openresty | 1.13.6.2 | [https://github.com/openresty/openresty/blob/master/doc/README-win32.md#readme](https://github.com/openresty/openresty/blob/master/doc/README-win32.md#readme) |
| openshift-origin-client | 3.11.0 | [https://www.openshift.org](https://www.openshift.org) |
| openssh | 7.6p1 | [https://www.openssh.com/](https://www.openssh.com/) |
| openssl-slp | 1.1.0j | [https://slproweb.com/products/Win32OpenSSL.html](https://slproweb.com/products/Win32OpenSSL.html) |
| openssl | 1.1.1a | [https://curl.haxx.se/windows/](https://curl.haxx.se/windows/) |
| opentrack | 2.3.10 | [https://github.com/opentrack/opentrack](https://github.com/opentrack/opentrack) |
| openvpn | 2.4.6-I602 | [https://openvpn.net/](https://openvpn.net/) |
| opera | 57.0.3098.91 | [https://www.opera.com/](https://www.opera.com/) |
| optipng | 0.7.7 | [http://optipng.sourceforge.net/](http://optipng.sourceforge.net/) |
| orca | 3.1.4000.1830 | [https://msdn.microsoft.com/en-us/library/windows/desktop/aa370557(v=vs.85).aspx](https://msdn.microsoft.com/en-us/library/windows/desktop/aa370557(v=vs.85).aspx) |
| outlook-google-calendar-sync | 2.7.7-alpha | [https://phw198.github.io/OutlookGoogleCalendarSync/](https://phw198.github.io/OutlookGoogleCalendarSync/) |
| oxipng | 2.1.8 | [https://github.com/shssoichiro/oxipng](https://github.com/shssoichiro/oxipng) |
| p4merge | 152.131.2139 | [https://www.perforce.com/](https://www.perforce.com/) |
| packer | 1.3.3 | [https://www.packer.io](https://www.packer.io) |
| paint.net | 4.1.5 | [https://www.getpaint.net/](https://www.getpaint.net/) |
| palemoon-portable | 28.2.2 | [https://www.palemoon.org/](https://www.palemoon.org/) |
| palemoon | 28.2.2 | [https://www.palemoon.org/](https://www.palemoon.org/) |
| pandoc-crossref | 0.3.4.0 | [https://hackage.haskell.org/package/pandoc-crossref](https://hackage.haskell.org/package/pandoc-crossref) |
| pandoc | 2.5 | [https://pandoc.org/](https://pandoc.org/) |
| papdesigner | 2.2.0.8.04 | [http://friedrich-folkmann.de/papdesigner/Hauptseite.html](http://friedrich-folkmann.de/papdesigner/Hauptseite.html) |
| patch | 2.6.1 | [http://www.mingw.org/wiki/MSYS](http://www.mingw.org/wiki/MSYS) |
| patheditor | 1.0 | [https://patheditor2.codeplex.com/](https://patheditor2.codeplex.com/) |
| pathod | 4.0.4 | [https://mitmproxy.org/](https://mitmproxy.org/) |
| pcem | 14 | [https://pcem-emulator.co.uk/](https://pcem-emulator.co.uk/) |
| pci-z | 2.0-2017.07.01 | [https://www.pci-z.com/](https://www.pci-z.com/) |
| pciutils | 3.5.5 | [https://eternallybored.org/misc/pciutils/](https://eternallybored.org/misc/pciutils/) |
| pcregrep | 10.20 | [https://pcre.org/](https://pcre.org/) |
| pdf2djvu | 0.9.8 | [https://jwilk.net/software/pdf2djvu](https://jwilk.net/software/pdf2djvu) |
| pdfsam | 3.3.7 | [https://github.com/torakiki/pdfsam](https://github.com/torakiki/pdfsam) |
| pdftk | 2.02 | [https://www.pdflabs.com/tools/pdftk-server/](https://www.pdflabs.com/tools/pdftk-server/) |
| peco | 0.5.3 | [https://github.com/peco/peco/](https://github.com/peco/peco/) |
| peerblock | 1.1.691 | [https://forums.peerblock.com/](https://forums.peerblock.com/) |
| pentaho-data-integration | 8.2.0.0-342 | [https://pentaho.sourceforge.io/](https://pentaho.sourceforge.io/) |
| perl | 5.28.1.1 | [http://strawberryperl.com](http://strawberryperl.com) |
| persepolis | 3.1.0 | [https://persepolisdm.github.io/](https://persepolisdm.github.io/) |
| pester | 4.4.3 | [https://github.com/pester/Pester](https://github.com/pester/Pester) |
| phantomjs | 2.1.1 | [http://phantomjs.org/](http://phantomjs.org/) |
| php-nts-xdebug | 2.6.1-7.2 | [https://xdebug.org/](https://xdebug.org/) |
| php-nts | 7.2.13 | [http://windows.php.net](http://windows.php.net) |
| php-xdebug | 2.6.1-7.2 | [https://xdebug.org/](https://xdebug.org/) |
| php | 7.2.13 | [http://windows.php.net](http://windows.php.net) |
| picard | 2.0.4 | [https://picard.musicbrainz.org/](https://picard.musicbrainz.org/) |
| picotorrent | 0.15.0 | [https://picotorrent.org](https://picotorrent.org) |
| pixie | 4.1 | [http://www.nattyware.com/pixie.php](http://www.nattyware.com/pixie.php) |
| pkg-config | 0.26-1 | [https://www.freedesktop.org/wiki/Software/pkg-config/](https://www.freedesktop.org/wiki/Software/pkg-config/) |
| plantuml | 1.2018.13 | [http://plantuml.com/](http://plantuml.com/) |
| png2html | 1.1 | [https://www.engr.mun.ca/~holden/png2html.html](https://www.engr.mun.ca/~holden/png2html.html) |
| png2jpeg | 1.0.1.7 | [http://passgenwin.sourceforge.net/abpage/projects.xhtml#png2jpeg](http://passgenwin.sourceforge.net/abpage/projects.xhtml#png2jpeg) |
| pngcrush | 1.8.11 | [https://pmt.sourceforge.io/pngcrush/](https://pmt.sourceforge.io/pngcrush/) |
| pngquant | 2.12.1 | [https://pngquant.org/](https://pngquant.org/) |
| poppler | 0.68.0 | [http://blog.alivate.com.au/poppler-windows/](http://blog.alivate.com.au/poppler-windows/) |
| portainer | 1.19.2 | [https://portainer.io/](https://portainer.io/) |
| posh-docker | 0.7.0 | [https://github.com/samneirinck/posh-docker](https://github.com/samneirinck/posh-docker) |
| posh-git | 0.7.1 | [http://dahlbyk.github.io/posh-git/](http://dahlbyk.github.io/posh-git/) |
| postgresql | 11.1 | [https://www.postgresql.org/](https://www.postgresql.org/) |
| postman | 6.6.1 | [https://www.getpostman.com/](https://www.getpostman.com/) |
| potrace | 1.15 | [http://potrace.sourceforge.net/](http://potrace.sourceforge.net/) |
| powerping | 1.2.0 | [https://github.com/Killeroo/PowerPing](https://github.com/Killeroo/PowerPing) |
| powertab | 1.1.0 | [https://github.com/jasonmarcher/PowerTab](https://github.com/jasonmarcher/PowerTab) |
| ppsspp | 1.7.4 | [https://www.ppsspp.org](https://www.ppsspp.org) |
| premake4 | 4.4-b5 | [https://premake.github.io/download.html](https://premake.github.io/download.html) |
| premake5 | 5.0.0-alpha13 | [https://premake.github.io/](https://premake.github.io/) |
| process-explorer | 16.22 | [https://docs.microsoft.com/en-us/sysinternals/downloads/process-explorer](https://docs.microsoft.com/en-us/sysinternals/downloads/process-explorer) |
| process-explorer64 | 16.22 | [https://docs.microsoft.com/en-us/sysinternals/downloads/process-explorer](https://docs.microsoft.com/en-us/sysinternals/downloads/process-explorer) |
| processhacker | 2.39 | [http://processhacker.sourceforge.net/](http://processhacker.sourceforge.net/) |
| procexp | 16.22 | [https://docs.microsoft.com/en-us/sysinternals/downloads/process-explorer](https://docs.microsoft.com/en-us/sysinternals/downloads/process-explorer) |
| procexp64 | 16.22 | [https://docs.microsoft.com/en-us/sysinternals/downloads/process-explorer](https://docs.microsoft.com/en-us/sysinternals/downloads/process-explorer) |
| prometheus | 2.5.0 | [https://prometheus.io/](https://prometheus.io/) |
| protobuf | 3.6.1 | [https://github.com/google/protobuf](https://github.com/google/protobuf) |
| proxifier-portable | 3.42 | [https://www.proxifier.com](https://www.proxifier.com) |
| psake | 4.7.4 | [https://github.com/psake/psake](https://github.com/psake/psake) |
| psgithub | 2017.01.22 | []() |
| pshazz | 0.2018.09.25 | [https://github.com/lukesampson/pshazz](https://github.com/lukesampson/pshazz) |
| psiphon3 | 136 | [https://s3.amazonaws.com/psiphon/web/60l3-nnss-6gsn/index.html](https://s3.amazonaws.com/psiphon/web/60l3-nnss-6gsn/index.html) |
| PSPad | 5.0.0 | [http://www.pspad.com](http://www.pspad.com) |
| psutils | 0.2018.08.04 | [https://github.com/lukesampson/psutils](https://github.com/lukesampson/psutils) |
| pt | 2.2.0 | [https://github.com/monochromegane/the_platinum_searcher](https://github.com/monochromegane/the_platinum_searcher) |
| pup | 0.4.0 | [https://github.com/ericchiang/pup](https://github.com/ericchiang/pup) |
| puppet | 5.5.8 | [https://puppetlabs.com](https://puppetlabs.com) |
| purescript | 0.12.1 | [http://purescript.org/](http://purescript.org/) |
| putty | 0.70 | [https://www.chiark.greenend.org.uk/~sgtatham/putty/](https://www.chiark.greenend.org.uk/~sgtatham/putty/) |
| pwsafe | 3.47.2 | [https://pwsafe.org/](https://pwsafe.org/) |
| pwsh | 6.1.1 | [https://github.com/PowerShell/PowerShell](https://github.com/PowerShell/PowerShell) |
| px | 2018-05-18 | [https://github.com/genotrance/px](https://github.com/genotrance/px) |
| pycharm | 2018.3.1 | [https://www.jetbrains.com/pycharm/](https://www.jetbrains.com/pycharm/) |
| pychess | 0.99.3 | [http://pychess.org/](http://pychess.org/) |
| pypy2 | 6.0.0 | [https://pypy.org](https://pypy.org) |
| python-exp | 3.5.2 | [https://www.python.org/](https://www.python.org/) |
| python | 3.7.1 | [https://www.python.org/](https://www.python.org/) |
| python27 | 2.7.15 | [https://www.python.org/](https://www.python.org/) |
| python35 | 3.5.4 | [https://www.python.org/](https://www.python.org/) |
| qaac | 2.68 | [https://sites.google.com/site/qaacpage/](https://sites.google.com/site/qaacpage/) |
| qbittorrent | 4.1.4 | [https://www.qbittorrent.org/](https://www.qbittorrent.org/) |
| qemu | 3.1.0 | [https://qemu.weilnetz.de/](https://qemu.weilnetz.de/) |
| qnapi | 0.2.3 | [https://qnapi.github.io/](https://qnapi.github.io/) |
| qpdf | 8.2.1 | [http://qpdf.sourceforge.net/](http://qpdf.sourceforge.net/) |
| qrencode | 3.4.4 | [https://code.google.com/archive/p/qrencode-win32/](https://code.google.com/archive/p/qrencode-win32/) |
| quicklook | 3.6.4 | [https://pooi.moe/QuickLook/](https://pooi.moe/QuickLook/) |
| quiterss | 0.18.12 | [https://quiterss.org/en](https://quiterss.org/en) |
| qutebrowser | 1.5.2 | [https://www.qutebrowser.org/](https://www.qutebrowser.org/) |
| r | 3.5.1 | [https://www.r-project.org](https://www.r-project.org) |
| rabbitmq | 3.7.9 | [https://www.rabbitmq.com/](https://www.rabbitmq.com/) |
| rabbitmqadmin | 3.7.9 | [https://www.rabbitmq.com/management-cli.html](https://www.rabbitmq.com/management-cli.html) |
| racket | 7.1 | [https://racket-lang.org](https://racket-lang.org) |
| radare2 | 3.1.3 | [https://www.radare.org/r/](https://www.radare.org/r/) |
| ragel | 6.9 | [https://github.com/eloraiby/ragel-windows](https://github.com/eloraiby/ragel-windows) |
| rainmeter | 4.2.0.3111 | [https://rainmeter.net/](https://rainmeter.net/) |
| rambox-pro | 1.0.8 | [https://rambox.pro/](https://rambox.pro/) |
| rambox | 0.6.3 | [http://rambox.pro/](http://rambox.pro/) |
| rancher-compose | 0.12.5 | [https://rancher.com/](https://rancher.com/) |
| rapidee | 937 | [https://www.rapidee.com/en/about](https://www.rapidee.com/en/about) |
| rcedit | 1.1.1 | [https://github.com/electron/rcedit](https://github.com/electron/rcedit) |
| rclone | 1.45 | [https://rclone.org](https://rclone.org) |
| reaper | 5.963 | [https://www.reaper.fm](https://www.reaper.fm) |
| recuva | 1.53.1087 | [https://www.ccleaner.com/recuva](https://www.ccleaner.com/recuva) |
| red | 0.6.4 | [http://www.red-lang.org](http://www.red-lang.org) |
| redis | 3.2.100 | [https://redis.io](https://redis.io) |
| renderdoc | 1.2 | [https://renderdoc.org](https://renderdoc.org) |
| reshade | 4.0.2 | [https://reshade.me/](https://reshade.me/) |
| resharper-clt | 2018.2.3 | [https://www.jetbrains.com/resharper/download/index.html#section=resharper-clt](https://www.jetbrains.com/resharper/download/index.html#section=resharper-clt) |
| resource-hacker | 5.1.6 | [http://www.angusj.com/resourcehacker/](http://www.angusj.com/resourcehacker/) |
| restic | 0.9.3 | [https://restic.github.io/](https://restic.github.io/) |
| rethinkdb | 2.3.6 | [https://www.rethinkdb.com/](https://www.rethinkdb.com/) |
| retroarch | 1.7.5 | [http://www.retroarch.com/](http://www.retroarch.com/) |
| ripgrep | 0.10.0 | [https://github.com/BurntSushi/ripgrep](https://github.com/BurntSushi/ripgrep) |
| ripme | 1.7.72 | [https://github.com/RipMeApp/ripme](https://github.com/RipMeApp/ripme) |
| rktools2k3 | 1.0 | [https://github.com/kodybrown/rktools2k3](https://github.com/kodybrown/rktools2k3) |
| robo3t | 1.2.1 | [https://robomongo.org](https://robomongo.org) |
| rstudio | 1.1.463 | [https://www.rstudio.com/](https://www.rstudio.com/) |
| rtmpdump | 2.3 | [https://rtmpdump.mplayerhq.hu/](https://rtmpdump.mplayerhq.hu/) |
| ruby | 2.4.5-1 | [https://rubyinstaller.org](https://rubyinstaller.org) |
| rufus | 3.4 | [https://rufus.ie/](https://rufus.ie/) |
| runat | 0.2018.08.04 | [https://github.com/lukesampson/psutils](https://github.com/lukesampson/psutils) |
| rust-msvc-nightly | nightly | [https://www.rust-lang.org](https://www.rust-lang.org) |
| rust-msvc | 1.30.1 | [https://www.rust-lang.org](https://www.rust-lang.org) |
| rust-nightly | nightly | [https://www.rust-lang.org](https://www.rust-lang.org) |
| rust | 1.30.1 | [https://www.rust-lang.org](https://www.rust-lang.org) |
| rustup | 1.16.0 | [https://github.com/rust-lang-nursery/rustup.rs](https://github.com/rust-lang-nursery/rustup.rs) |
| rxrepl | 1.5 | [https://sites.google.com/site/regexreplace/](https://sites.google.com/site/regexreplace/) |
| s | 0.5.13 | [https://github.com/zquestz/s](https://github.com/zquestz/s) |
| s3deploy | 2.2.0 | []() |
| sabnzbd | 2.3.5 | [https://sabnzbd.org/](https://sabnzbd.org/) |
| sacad | 2.1.7 | [https://github.com/desbma/sacad](https://github.com/desbma/sacad) |
| sandman | 1.9.2 | [https://alexanderepstein.github.io/Sandman/](https://alexanderepstein.github.io/Sandman/) |
| sass | 1.15.2 | [https://github.com/sass/dart-sass](https://github.com/sass/dart-sass) |
| say | 0.2018.08.04 | [https://github.com/lukesampson/psutils](https://github.com/lukesampson/psutils) |
| sbcl | 1.4.14 | [http://www.sbcl.org/](http://www.sbcl.org/) |
| sbt | 1.2.7 | [https://www.scala-sbt.org/](https://www.scala-sbt.org/) |
| scala | 2.12.8 | [https://www.scala-lang.org/](https://www.scala-lang.org/) |
| scallion | 2.1 | [https://github.com/lachesis/scallion](https://github.com/lachesis/scallion) |
| scholdoc | 0.1.3 | [http://scholdoc.scholarlymarkdown.com/](http://scholdoc.scholarlymarkdown.com/) |
| scons | 3.0.1 | [https://scons.org/](https://scons.org/) |
| scrcpy | 1.5 | [https://github.com/Genymobile/scrcpy](https://github.com/Genymobile/scrcpy) |
| screentogif | 2.14.1 | [http://www.screentogif.com/](http://www.screentogif.com/) |
| scriptcs | 0.17.1 | [http://scriptcs.net/](http://scriptcs.net/) |
| sdl2 | 2.0.7 | [https://www.libsdl.org](https://www.libsdl.org) |
| sed | 4.2.1 | [http://gnuwin32.sourceforge.net/packages/sed.htm](http://gnuwin32.sourceforge.net/packages/sed.htm) |
| selenium | 3.141.59 | [http://www.seleniumhq.org/](http://www.seleniumhq.org/) |
| sendemail | 156 | [http://caspian.dotconf.net/menu/Software/SendEmail/](http://caspian.dotconf.net/menu/Software/SendEmail/) |
| seqcli | 5.0.165 | [https://github.com/datalust/seqcli](https://github.com/datalust/seqcli) |
| serve | 0.2.1 | [https://github.com/philippgille/serve](https://github.com/philippgille/serve) |
| servicebusexplorer | 4.0.110 | [https://github.com/paolosalvatori/ServiceBusExplorer](https://github.com/paolosalvatori/ServiceBusExplorer) |
| sfk | 1.9.3.4 | [http://stahlworks.com/dev/swiss-file-knife.html](http://stahlworks.com/dev/swiss-file-knife.html) |
| shadowsocks | 4.1.2 | [https://github.com/shadowsocks/shadowsocks-windows](https://github.com/shadowsocks/shadowsocks-windows) |
| shadowsocksr-csharp | 4.9.0 | [https://github.com/shadowsocksrr/shadowsocksr-csharp](https://github.com/shadowsocksrr/shadowsocksr-csharp) |
| sharex | 12.3.1 | [https://getsharex.com/](https://getsharex.com/) |
| sharpkeys | 3.8 | [https://github.com/randyrants/sharpkeys](https://github.com/randyrants/sharpkeys) |
| shasum | 0.2018.08.04 | [https://github.com/lukesampson/psutils](https://github.com/lukesampson/psutils) |
| shellcheck | 0.6.0 | [https://shellcheck.net/](https://shellcheck.net/) |
| shim | 0.2013.11.19 | [https://github.com/lukesampson/psutils](https://github.com/lukesampson/psutils) |
| shinjiru | 3.3.2 | [https://shinjiru.me/](https://shinjiru.me/) |
| signal | 1.19.0 | [https://signal.org/](https://signal.org/) |
| simplewall | 2.3.10 | [https://www.henrypp.org/product/simplewall](https://www.henrypp.org/product/simplewall) |
| skaffold | 0.19.0 | [https://github.com/GoogleCloudPlatform/skaffold](https://github.com/GoogleCloudPlatform/skaffold) |
| slack | 3.3.3 | [https://slack.com/downloads/windows](https://slack.com/downloads/windows) |
| sliksvn | 1.9.7 | [https://sliksvn.com/](https://sliksvn.com/) |
| smartmontools | 6.6-1 | [https://www.smartmontools.org/](https://www.smartmontools.org/) |
| smartty | 3.1 | [http://smartty.sysprogs.com/](http://smartty.sysprogs.com/) |
| snaketail | 1.9.4 | [http://snakenest.com/snaketail/](http://snakenest.com/snaketail/) |
| snipaste | 1.16.2 | [https://www.snipaste.com/](https://www.snipaste.com/) |
| soapui | 5.4.0 | [https://www.soapui.org/](https://www.soapui.org/) |
| solidity | 0.5.1 | [https://solidity.readthedocs.io](https://solidity.readthedocs.io) |
| sonarqube | 7.4 | [https://www.sonarqube.org](https://www.sonarqube.org) |
| soulseekqt | 2017-2-20 | [http://www.slsknet.org/news/node/1](http://www.slsknet.org/news/node/1) |
| sourcetree | 3.0.12 | [https://www.sourcetreeapp.com/](https://www.sourcetreeapp.com/) |
| SpaceSniffer | 1.3.0.2 | [http://www.uderzo.it/main_products/space_sniffer/index.html](http://www.uderzo.it/main_products/space_sniffer/index.html) |
| spark | 2.4.0 | [https://spark.apache.org/](https://spark.apache.org/) |
| speccy | 1.32.740 | [https://www.piriform.com/speccy](https://www.piriform.com/speccy) |
| speedcrunch | 0.12 | [http://speedcrunch.org/](http://speedcrunch.org/) |
| speedfan | 4.52 | [http://www.almico.com/speedfan.php](http://www.almico.com/speedfan.php) |
| speedyfox | 2.0.25 | [https://www.crystalidea.com/speedyfox](https://www.crystalidea.com/speedyfox) |
| springboot | 2.1.1 | [https://projects.spring.io/spring-boot/](https://projects.spring.io/spring-boot/) |
| spytify | 1.1.3.1 | [https://github.com/jwallet/spy-spotify](https://github.com/jwallet/spy-spotify) |
| sqlite | 3.26.0 | [https://www.sqlite.org/](https://www.sqlite.org/) |
| sqlitebrowser | 3.10.1 | [http://sqlitebrowser.org/](http://sqlitebrowser.org/) |
| sqlitestudio | 3.2.1 | [https://sqlitestudio.pl/index.rvt](https://sqlitestudio.pl/index.rvt) |
| sqlopsstudio | 0.33.7 | [https://docs.microsoft.com/en-us/sql/sql-operations-studio](https://docs.microsoft.com/en-us/sql/sql-operations-studio) |
| squashfs-tools | 43 | [https://github.com/pmq20/squashfuse](https://github.com/pmq20/squashfuse) |
| srvman | 1.0 | [http://tools.sysprogs.org/srvman/](http://tools.sysprogs.org/srvman/) |
| ssd-z | 16.09.09 | [http://aezay.dk/aezay/ssdz/](http://aezay.dk/aezay/ssdz/) |
| ssh-copy-id | 2015-03-22 | [https://github.com/VijayS1/Scripts/blob/master/ssh-copy-id/README.md](https://github.com/VijayS1/Scripts/blob/master/ssh-copy-id/README.md) |
| sslscan | 1.11.11 | [https://github.com/rbsec/sslscan](https://github.com/rbsec/sslscan) |
| stack | 1.9.3 | [https://www.haskellstack.org](https://www.haskellstack.org) |
| station | 1.31.3 | [https://getstation.com/](https://getstation.com/) |
| steam-library-manager | 1.5.0.12 | [https://github.com/RevoLand/Steam-Library-Manager](https://github.com/RevoLand/Steam-Library-Manager) |
| steam | nightly | [https://store.steampowered.com/](https://store.steampowered.com/) |
| steamcmd | 1532461524 | [https://developer.valvesoftware.com/wiki/SteamCMD](https://developer.valvesoftware.com/wiki/SteamCMD) |
| stone-soup-tiles | 0.22.1 | [https://crawl.develz.org/](https://crawl.develz.org/) |
| stone-soup | 0.22.1 | [https://crawl.develz.org/](https://crawl.develz.org/) |
| storageexplorer | 1.5.0 | [https://azure.microsoft.com/en-us/features/storage-explorer/](https://azure.microsoft.com/en-us/features/storage-explorer/) |
| streamlink | 0.14.2 | [https://streamlink.github.io/](https://streamlink.github.io/) |
| strokesplus-portable | 2.8.6.4 | [https://www.strokesplus.com](https://www.strokesplus.com) |
| sts | 3.9.6 | [https://spring.io/tools/sts](https://spring.io/tools/sts) |
| stunnel | 5.49 | [https://www.stunnel.org](https://www.stunnel.org) |
| sublime-merge | 1097 | [https://www.sublimemerge.com/](https://www.sublimemerge.com/) |
| sublime-text | 3176 | [https://www.sublimetext.com/3](https://www.sublimetext.com/3) |
| subtitleedit | 3.5.7 | [http://www.nikse.dk/subtitleedit/](http://www.nikse.dk/subtitleedit/) |
| sudo | 0.2018.08.04 | [https://github.com/lukesampson/psutils](https://github.com/lukesampson/psutils) |
| sumatrapdf | 3.1.2 | [https://www.sumatrapdfreader.org](https://www.sumatrapdfreader.org) |
| sunsetscreen | 1.30 | [http://www.skytopia.com/software/sunsetscreen/](http://www.skytopia.com/software/sunsetscreen/) |
| svcat | 0.1.38 | [https://svc-cat.io/](https://svc-cat.io/) |
| svtplay-dl | 2.1 | [https://svtplay-dl.se/](https://svtplay-dl.se/) |
| sweethome3d | 6.0 | [http://www.sweethome3d.com/](http://www.sweethome3d.com/) |
| swig | 3.0.12 | [http://www.swig.org](http://www.swig.org) |
| syncany-cli | 0.4.9 | [https://www.syncany.org/](https://www.syncany.org/) |
| syncbackpro | 8.5.97.0 | [https://www.2brightsparks.com/syncback/sbpro.html](https://www.2brightsparks.com/syncback/sbpro.html) |
| syncthing | 0.14.54 | [https://syncthing.net/](https://syncthing.net/) |
| synctrayzor | 1.1.22 | [https://github.com/canton7/SyncTrayzor](https://github.com/canton7/SyncTrayzor) |
| sysinternals | July.5.2018 | [https://docs.microsoft.com/en-us/sysinternals/](https://docs.microsoft.com/en-us/sysinternals/) |
| taiga | 1.3.1 | [http://taiga.moe/](http://taiga.moe/) |
| tar | 1.23 | [http://www.mingw.org/wiki/msys](http://www.mingw.org/wiki/msys) |
| task | 2.2.1 | [https://taskfile.org](https://taskfile.org) |
| tcc | 0.9.26 | [https://bellard.org/tcc/](https://bellard.org/tcc/) |
| tcpipmanager | 4.1.1 | [http://tcpipmanager.sourceforge.net](http://tcpipmanager.sourceforge.net) |
| teamspeak3 | 3.2.3 | [https://www.teamspeak.com/en/](https://www.teamspeak.com/en/) |
| teamviewer | 14.0.13880 | [https://www.teamviewer.com](https://www.teamviewer.com) |
| telegram | 1.5.1 | [https://telegram.org/](https://telegram.org/) |
| telnet | msys-inetutils-1.7-1 | [http://www.mingw.org/wiki/msys](http://www.mingw.org/wiki/msys) |
| terminals | 4.0.1 | [https://github.com/Terminals-Origin/Terminals](https://github.com/Terminals-Origin/Terminals) |
| terminus | 1.0.65 | [https://eugeny.github.io/terminus/](https://eugeny.github.io/terminus/) |
| terraform | 0.11.10 | [https://www.terraform.io](https://www.terraform.io) |
| terragrunt | 0.17.3 | [https://github.com/gruntwork-io/terragrunt](https://github.com/gruntwork-io/terragrunt) |
| tesseract | 4.0.0.20181030 | [https://github.com/UB-Mannheim/tesseract/wiki](https://github.com/UB-Mannheim/tesseract/wiki) |
| texmaker | 5.0.3 | [http://www.xm1math.net/texmaker/](http://www.xm1math.net/texmaker/) |
| texstudio | 2.12.14 | [https://www.texstudio.org](https://www.texstudio.org) |
| textadept | 10.2 | [https://foicica.com/textadept/](https://foicica.com/textadept/) |
| texteditoranywhere | 2.01 | [https://www.listary.com/text-editor-anywhere](https://www.listary.com/text-editor-anywhere) |
| thrift | 0.11.0 | [https://thrift.apache.org/](https://thrift.apache.org/) |
| thunderbird | 60.3.3 | [https://www.mozilla.org/en-US/thunderbird/](https://www.mozilla.org/en-US/thunderbird/) |
| tidy | 5.6.0 | [http://www.html-tidy.org/](http://www.html-tidy.org/) |
| time | 0.2018.08.04 | [https://github.com/lukesampson/psutils](https://github.com/lukesampson/psutils) |
| todolist | 7.1.5.0 | [https://abstractspoon.weebly.com/](https://abstractspoon.weebly.com/) |
| tomcat | 9.0.12 | [https://tomcat.apache.org/](https://tomcat.apache.org/) |
| tor-browser | 8.0.4 | [https://www.torproject.org/](https://www.torproject.org/) |
| tor-expert | 0.3.4.9 | [https://www.torproject.org](https://www.torproject.org) |
| tortoisemerge | 1.6.7 | [https://tortoisesvn.net/TortoiseMerge.html](https://tortoisesvn.net/TortoiseMerge.html) |
| tortoisesvn | 1.11.0.28416 | [https://tortoisesvn.net](https://tortoisesvn.net) |
| totalcommander | 9.21a | [https://www.ghisler.com](https://www.ghisler.com) |
| touch | 0.2018.08.04 | [https://github.com/lukesampson/psutils](https://github.com/lukesampson/psutils) |
| traefik | 1.7.5 | [https://traefik.io/](https://traefik.io/) |
| transmission-cli | 2.94 | [https://transmissionbt.com/](https://transmissionbt.com/) |
| transmission | 2.94 | [https://transmissionbt.com/](https://transmissionbt.com/) |
| tremulous | 1.3.0-alpha.0.13 | [http://tremulous.net/](http://tremulous.net/) |
| trid | 2.24-18.12.11 | [http://mark0.net/soft-trid-e.html](http://mark0.net/soft-trid-e.html) |
| tunnel | 0.2.12 | [https://github.com/labstack/tunnel-client](https://github.com/labstack/tunnel-client) |
| tup | 0.7.8 | [http://gittup.org](http://gittup.org) |
| UIforETW | 1.50 | [https://github.com/google/UIforETW](https://github.com/google/UIforETW) |
| unar | 1.8.1 | [https://theunarchiver.com/command-line](https://theunarchiver.com/command-line) |
| unbound | 1.8.3 | [https://unbound.net/](https://unbound.net/) |
| uncap | 0.2.2 | [https://github.com/susam/uncap](https://github.com/susam/uncap) |
| uncrustify | 0.68.1 | [http://uncrustify.sourceforge.net/](http://uncrustify.sourceforge.net/) |
| unetbootin | 661 | [https://unetbootin.github.io](https://unetbootin.github.io) |
| ungoogled-chromium | 67.0.3396.87-3 | [https://github.com/Eloston/ungoogled-chromium](https://github.com/Eloston/ungoogled-chromium) |
| universalpausebutton | 1.0.3 | [https://github.com/ryanries/UniversalPauseButton](https://github.com/ryanries/UniversalPauseButton) |
| unlocker | 1.9.0 | [http://www.emptyloop.com/unlocker](http://www.emptyloop.com/unlocker) |
| unrar | 5.61 | [https://www.rarlab.com/](https://www.rarlab.com/) |
| unzip | 6.00 | [http://www.info-zip.org/](http://www.info-zip.org/) |
| up | 0.8.1 | [https://github.com/apex/up](https://github.com/apex/up) |
| upx | 3.95 | [https://upx.github.io/](https://upx.github.io/) |
| usql | 0.7.0 | [https://github.com/xo/usql](https://github.com/xo/usql) |
| util-linux-ng | 2.14.1 | [http://gnuwin32.sourceforge.net/packages/util-linux-ng.htm](http://gnuwin32.sourceforge.net/packages/util-linux-ng.htm) |
| vagrant | 2.2.2 | [https://www.vagrantup.com/](https://www.vagrantup.com/) |
| vault | 1.0.0 | [https://www.vaultproject.io](https://www.vaultproject.io) |
| vbindiff | 3.0-beta5 | [https://www.cjmweb.net/vbindiff/](https://www.cjmweb.net/vbindiff/) |
| vcredist | 14.10.25008 | [https://www.visualstudio.com/de/downloads/](https://www.visualstudio.com/de/downloads/) |
| vcredist2008 | 9.0.30729 | [https://support.microsoft.com/en-us/help/2977003/the-latest-supported-visual-c-downloads](https://support.microsoft.com/en-us/help/2977003/the-latest-supported-visual-c-downloads) |
| vcredist2010 | 10.0.40219 | [https://support.microsoft.com/en-us/help/2977003/the-latest-supported-visual-c-downloads](https://support.microsoft.com/en-us/help/2977003/the-latest-supported-visual-c-downloads) |
| vcredist2012 | 11.0.61030 | [https://support.microsoft.com/en-us/help/2977003/the-latest-supported-visual-c-downloads](https://support.microsoft.com/en-us/help/2977003/the-latest-supported-visual-c-downloads) |
| vcredist2013 | 12.0.40660 | [https://support.microsoft.com/en-us/help/2977003/the-latest-supported-visual-c-downloads](https://support.microsoft.com/en-us/help/2977003/the-latest-supported-visual-c-downloads) |
| vcredist2015 | 14.0.24215 | [https://support.microsoft.com/en-us/help/2977003/the-latest-supported-visual-c-downloads](https://support.microsoft.com/en-us/help/2977003/the-latest-supported-visual-c-downloads) |
| vcredist2017 | 14.10.25008 | [https://www.visualstudio.com/de/downloads/](https://www.visualstudio.com/de/downloads/) |
| vcxsrv | 1.20.1.4 | [https://vcxsrv.sourceforge.io/](https://vcxsrv.sourceforge.io/) |
| vifm | 0.10 | [https://vifm.info/](https://vifm.info/) |
| vim | 8.1.0577 | [http://www.vim.org](http://www.vim.org) |
| vimtutor | 0.2018.08.04 | [https://github.com/lukesampson/psutils](https://github.com/lukesampson/psutils) |
| visual-arm-emulator | 1.27 | [https://salmanarif.bitbucket.io/visual/index.html](https://salmanarif.bitbucket.io/visual/index.html) |
| visualc | 16.00.30319.01 | [https://www.visualstudio.com](https://www.visualstudio.com) |
| vivaldi | 2.1.1337.51 | [https://vivaldi.com/](https://vivaldi.com/) |
| vlc | 3.0.4 | [https://www.videolan.org/](https://www.videolan.org/) |
| vncviewer | 6.18.907 | [https://www.realvnc.com/download/viewer](https://www.realvnc.com/download/viewer) |
| vnote | 2.1 | [https://tamlok.github.io/vnote/](https://tamlok.github.io/vnote/) |
| vott | 1.7.1 | [https://github.com/Microsoft/VoTT](https://github.com/Microsoft/VoTT) |
| vscode-insiders-portable | nightly | [https://code.visualstudio.com/](https://code.visualstudio.com/) |
| vscode-insiders | nightly | [https://code.visualstudio.com/](https://code.visualstudio.com/) |
| vscode-portable | 1.29.1 | [https://code.visualstudio.com/](https://code.visualstudio.com/) |
| vscode | 1.29.1 | [https://code.visualstudio.com/](https://code.visualstudio.com/) |
| vswhere | 2.5.2 | [https://github.com/Microsoft/vswhere](https://github.com/Microsoft/vswhere) |
| warp | 0.3.0 | [https://github.com/dgiagio/warp](https://github.com/dgiagio/warp) |
| watchexec | 1.9.2 | [https://github.com/mattgreen/watchexec](https://github.com/mattgreen/watchexec) |
| watchman-nightly | nightly | [https://facebook.github.io/watchman/](https://facebook.github.io/watchman/) |
| wavebox | 4.5.5 | [https://wavebox.io/](https://wavebox.io/) |
| webpicmd | 4.5 | [https://docs.microsoft.com/en-us/iis/install/web-platform-installer/web-platform-installer-v4-command-line-webpicmdexe-rtw-release](https://docs.microsoft.com/en-us/iis/install/web-platform-installer/web-platform-installer-v4-command-line-webpicmdexe-rtw-release) |
| webstorm | 2018.3.1 | [https://www.jetbrains.com/webstorm/](https://www.jetbrains.com/webstorm/) |
| webtorrent | 0.20.0 | [https://webtorrent.io/desktop/](https://webtorrent.io/desktop/) |
| wget | 1.20 | [https://eternallybored.org/misc/wget/](https://eternallybored.org/misc/wget/) |
| whatsapp | 0.3.1649 | [https://www.whatsapp.com](https://www.whatsapp.com) |
| which | 2.20 | [http://gnuwin32.sourceforge.net/packages/which.htm](http://gnuwin32.sourceforge.net/packages/which.htm) |
| wifi-manager | 0.2 | [https://github.com/shanselman/Windows-Wifi-Manager](https://github.com/shanselman/Windows-Wifi-Manager) |
| win-acme | 1.9.12.2 | [https://github.com/PKISharp/win-acme](https://github.com/PKISharp/win-acme) |
| win-portacle | 1.2c | [https://portacle.github.io/](https://portacle.github.io/) |
| win32-disk-imager | 1.0.0 | [https://sourceforge.net/projects/win32diskimager/](https://sourceforge.net/projects/win32diskimager/) |
| win32-openssh | 7.7.2.0p1-Beta | [https://github.com/PowerShell/Win32-OpenSSH](https://github.com/PowerShell/Win32-OpenSSH) |
| winbox | 3.18 | [https://mikrotik.com/](https://mikrotik.com/) |
| wincdemu | 4.0 | [http://wincdemu.sysprogs.org/](http://wincdemu.sysprogs.org/) |
| wincompose | 0.8.2 | [http://wincompose.info/](http://wincompose.info/) |
| windirstat | 1.1.2 | [https://windirstat.net/](https://windirstat.net/) |
| windows-application-driver | 1.1 | [https://github.com/Microsoft/WinAppDriver](https://github.com/Microsoft/WinAppDriver) |
| winfile-original | 10.0 | [https://github.com/Microsoft/winfile](https://github.com/Microsoft/winfile) |
| winfile | 10.0.1806.1 | [https://github.com/Microsoft/winfile](https://github.com/Microsoft/winfile) |
| winmerge | 2.16.0 | [http://winmerge.org](http://winmerge.org) |
| winmerge2011 | 0.2011.008.313 | [https://bitbucket.org/jtuc/winmerge2011](https://bitbucket.org/jtuc/winmerge2011) |
| winpython | 3.6.7.0 | [https://winpython.github.io/](https://winpython.github.io/) |
| winrar | 5.61 | [https://rarlab.com/](https://rarlab.com/) |
| winscp | 5.13.6 | [https://winscp.net](https://winscp.net) |
| winyl | 3.3.1 | [http://vinylsoft.com/](http://vinylsoft.com/) |
| wireshark | 2.6.5 | [https://www.wireshark.org/](https://www.wireshark.org/) |
| wixtoolset | 3.11.1 | [http://wixtoolset.org/](http://wixtoolset.org/) |
| wiztree | 3.26 | [https://antibody-software.com/web/software/software/wiztree-finds-the-files-and-folders-using-the-most-disk-space-on-your-hard-drive](https://antibody-software.com/web/software/software/wiztree-finds-the-files-and-folders-using-the-most-disk-space-on-your-hard-drive) |
| wkhtmltopdf | 0.12.5-1 | [https://wkhtmltopdf.org/](https://wkhtmltopdf.org/) |
| wox | 1.3.524 | [http://www.wox.one/](http://www.wox.one/) |
| write | 1.0b8.4 | [https://wri.tt/](https://wri.tt/) |
| wsltty | 1.9.5 | [https://github.com/mintty/wsltty](https://github.com/mintty/wsltty) |
| wurl | 1.0.1 | [https://github.com/xakep666/wurl](https://github.com/xakep666/wurl) |
| wuzz | 0.4.0 | [https://github.com/asciimoo/wuzz](https://github.com/asciimoo/wuzz) |
| wxhexeditor | 0.24 | [http://www.wxhexeditor.org/](http://www.wxhexeditor.org/) |
| wyam | 2.1.0 | [https://wyam.io](https://wyam.io) |
| x264-10bit | 2851 | [https://www.videolan.org/developers/x264.html](https://www.videolan.org/developers/x264.html) |
| x264 | 2935 | [https://www.videolan.org/developers/x264.html](https://www.videolan.org/developers/x264.html) |
| x64dbg | 2018-11-27_12-40 | [https://x64dbg.com/](https://x64dbg.com/) |
| xdelta | 3.1.0 | [http://xdelta.org/](http://xdelta.org/) |
| xdman | 7.2.8 | [http://xdman.sourceforge.net/](http://xdman.sourceforge.net/) |
| xmake | 2.2.3 | [https://xmake.io](https://xmake.io) |
| xmedia-recode | 3.4.4.8 | [https://www.xmedia-recode.de/en/](https://www.xmedia-recode.de/en/) |
| xmind8 | 3.7.8 | [https://www.xmind.net/](https://www.xmind.net/) |
| xming | 6.9.0.31 | [http://www.straightrunning.com/XmingNotes/](http://www.straightrunning.com/XmingNotes/) |
| xmllint | 2.9.3 | [http://xmlsoft.org/](http://xmlsoft.org/) |
| xmlstarlet | 1.6.1 | [http://xmlstar.sourceforge.net/](http://xmlstar.sourceforge.net/) |
| xmousebuttoncontrol | 2.17 | [https://www.highrez.co.uk/downloads/xmousebuttoncontrol.htm](https://www.highrez.co.uk/downloads/xmousebuttoncontrol.htm) |
| xsv | 0.13.0 | [https://github.com/BurntSushi/xsv](https://github.com/BurntSushi/xsv) |
| xx-net | 3.12.11 | [https://github.com/XX-net/XX-Net](https://github.com/XX-net/XX-Net) |
| xyplorer | 17.40.0100 | [https://www.xyplorer.com/free.php](https://www.xyplorer.com/free.php) |
| xz | 5.2.4 | [https://tukaani.org/xz/](https://tukaani.org/xz/) |
| yara | 3.8.1 | [https://virustotal.github.io/yara/](https://virustotal.github.io/yara/) |
| yarn | 1.12.3 | [https://yarnpkg.com/](https://yarnpkg.com/) |
| yasm | 1.3.0 | [http://yasm.tortall.net/](http://yasm.tortall.net/) |
| yatqa | 3.9.5 | [http://yat.qa/](http://yat.qa/) |
| youtube-dl-gui | 0.4 | [https://github.com/MrS0m30n3/youtube-dl-gui](https://github.com/MrS0m30n3/youtube-dl-gui) |
| youtube-dl | 2018.12.09 | [https://rg3.github.io/youtube-dl/](https://rg3.github.io/youtube-dl/) |
| yubico-piv-tool | 1.6.2 | [https://developers.yubico.com/yubico-piv-tool/](https://developers.yubico.com/yubico-piv-tool/) |
| yubikey-manager-qt | 0.5.2 | [https://developers.yubico.com/yubikey-manager-qt/](https://developers.yubico.com/yubikey-manager-qt/) |
| yubikey-personalization-gui | 3.1.25 | [https://developers.yubico.com/yubikey-personalization-gui/](https://developers.yubico.com/yubikey-personalization-gui/) |
| yubikey-personalization | 1.19.0 | [https://developers.yubico.com/yubikey-personalization/](https://developers.yubico.com/yubikey-personalization/) |
| yubikey-piv-manager | 1.4.2 | [https://developers.yubico.com/yubikey-piv-manager/](https://developers.yubico.com/yubikey-piv-manager/) |
| zeal | 0.6.1 | [https://zealdocs.org/](https://zealdocs.org/) |
| zeppelin | 0.8.0 | [https://zeppelin.apache.org/](https://zeppelin.apache.org/) |
| zeronet | 0.6.4 | [https://zeronet.io/](https://zeronet.io/) |
| ziglang | 0.3.0 | [https://ziglang.org/](https://ziglang.org/) |
| zip | 3.0 | [http://www.info-zip.org/](http://www.info-zip.org/) |
| zlocation | 1.1.0 | [https://github.com/vors/ZLocation](https://github.com/vors/ZLocation) |
| zola | 0.5.0 | [https://www.getzola.org/](https://www.getzola.org/) |
| zookeeper | 3.4.13 | [https://zookeeper.apache.org/](https://zookeeper.apache.org/) |
| zstd | 1.3.7 | [http://www.zstd.net/](http://www.zstd.net/) |

This file was automatically generated.
### List of apps in bucket
---
Automatically generated by the bin/build.ps1 script

| Name | Version | Homepage |
| ---- | ------- | -------- |
| 3rvx | 2.9.2 | [https://3rvx.com/](https://3rvx.com/) |
| 7zip | 18.05 | [http://www.7-zip.org/](http://www.7-zip.org/) |
| ack | 2.24 | [https://beyondgrep.com/](https://beyondgrep.com/) |
| acmesharp | 0.8.1.0 | [https://github.com/ebekker/ACMESharp](https://github.com/ebekker/ACMESharp) |
| adb | 28.0.1 | [https://developer.android.com/studio/releases/platform-tools.html](https://developer.android.com/studio/releases/platform-tools.html) |
| advancedrenamer | 3.84 | [https://www.advancedrenamer.com](https://www.advancedrenamer.com) |
| ag | 2.2.0-4-g1b06a9f | [https://geoff.greer.fm/ag/](https://geoff.greer.fm/ag/) |
| ahoy | 2.0.0 | [http://ahoycli.com](http://ahoycli.com) |
| aida64extreme | 5.99 | [https://www.aida64.com](https://www.aida64.com) |
| alacritty | 0.2.3 | [https://github.com/jwilm/alacritty/releases](https://github.com/jwilm/alacritty/releases) |
| allure | 2.8.1 | [https://github.com/allure-framework/allure2](https://github.com/allure-framework/allure2) |
| altools | 1.0 | [https://www.microsoft.com/en-us/download/details.aspx?id=18465](https://www.microsoft.com/en-us/download/details.aspx?id=18465) |
| ammonite | 1.5.0 | [http://ammonite.io](http://ammonite.io) |
| anaconda3 | 5.3.1 | [https://www.anaconda.com/](https://www.anaconda.com/) |
| android-sdk | 4333796 | [https://developer.android.com/studio/](https://developer.android.com/studio/) |
| android-studio | 3.2.1.0 | [https://developer.android.com/studio/](https://developer.android.com/studio/) |
| anki | 2.1.6 | [https://apps.ankiweb.net/](https://apps.ankiweb.net/) |
| annie | 0.8.5 | [https://github.com/iawia002/annie](https://github.com/iawia002/annie) |
| ant | 1.10.5 | [https://ant.apache.org/](https://ant.apache.org/) |
| antimicro | 2.23 | [https://github.com/AntiMicro/antimicro](https://github.com/AntiMicro/antimicro) |
| anydesk | 4.2.3 | [https://anydesk.com/](https://anydesk.com/) |
| apache-directory-studio | 2.0.0-M14 | [http://directory.apache.org/studio/](http://directory.apache.org/studio/) |
| apache-ivy | 2.4.0 | [https://ant.apache.org/ivy/index.html](https://ant.apache.org/ivy/index.html) |
| apache | 2.4.37 | [https://www.apachelounge.com](https://www.apachelounge.com) |
| apex | 1.0.0-rc3 | [http://apex.run/](http://apex.run/) |
| apngasm | 3.0.0 | [https://github.com/apngasm/apngasm](https://github.com/apngasm/apngasm) |
| appengine-go | 1.9.70 | [https://developers.google.com/appengine/](https://developers.google.com/appengine/) |
| archi | 4.3.1 | [https://www.archimatetool.com/](https://www.archimatetool.com/) |
| archwsl | 18120900 | [https://github.com/yuk7/ArchWSL/](https://github.com/yuk7/ArchWSL/) |
| arduino | 1.8.8 | [https://www.arduino.cc/](https://www.arduino.cc/) |
| aria2 | 1.34.0-1 | [https://aria2.github.io/](https://aria2.github.io/) |
| armclient | 1.3 | [https://github.com/projectkudu/ARMClient](https://github.com/projectkudu/ARMClient) |
| armor | 0.4.12 | [https://github.com/labstack/armor](https://github.com/labstack/armor) |
| artifact | 1.0.1 | [https://github.com/vitiral/artifact](https://github.com/vitiral/artifact) |
| assume-role | 0.3.2 | [https://github.com/remind101/assume-role](https://github.com/remind101/assume-role) |
| astrogrep | 4.4.6 | [http://astrogrep.sourceforge.net/](http://astrogrep.sourceforge.net/) |
| astyle | 3.1 | [http://astyle.sourceforge.net/](http://astyle.sourceforge.net/) |
| atom | 1.33.0 | [https://atom.io/](https://atom.io/) |
| atomicparsley | 0.9.0 | [http://atomicparsley.sourceforge.net/](http://atomicparsley.sourceforge.net/) |
| audacity | 2.3.0 | [https://www.audacityteam.org/](https://www.audacityteam.org/) |
| autohotkey-installer | 1.1.30.01 | [https://www.autohotkey.com/](https://www.autohotkey.com/) |
| autohotkey | 1.1.30.01 | [https://www.autohotkey.com/](https://www.autohotkey.com/) |
| autoit | 3.3.14.5 | [https://www.autoitscript.com/site/autoit/](https://www.autoitscript.com/site/autoit/) |
| awake | 1.4.2 | [https://github.com/gdegeneve/Awake](https://github.com/gdegeneve/Awake) |
| aws | 1.16.73 | [https://aws.amazon.com/cli/](https://aws.amazon.com/cli/) |
| axel | 2.4 | [https://github.com/ghuntley/cygwin-axel/](https://github.com/ghuntley/cygwin-axel/) |
| axis | 1.4 | [https://axis.apache.org/](https://axis.apache.org/) |
| azure-cli | 2.0.52 | [https://aka.ms/cli](https://aka.ms/cli) |
| azure-functions-core-tools | 2.3.148 | [https://github.com/Azure/azure-functions-core-tools](https://github.com/Azure/azure-functions-core-tools) |
| azure-ps | 6.13.1.24243 | [https://aka.ms/azpsdocs](https://aka.ms/azpsdocs) |
| azuredatastudio-insiders | 1.2.4 | [https://docs.microsoft.com/en-us/sql/azure-data-studio](https://docs.microsoft.com/en-us/sql/azure-data-studio) |
| azuredatastudio | 1.2.4 | [https://docs.microsoft.com/en-us/sql/azure-data-studio](https://docs.microsoft.com/en-us/sql/azure-data-studio) |
| baka-mplayer | 2.0.4 | [http://bakamplayer.u8sand.net/](http://bakamplayer.u8sand.net/) |
| bandizip | 6.18 | [http://www.bandisoft.com/bandizip/](http://www.bandisoft.com/bandizip/) |
| baretail | 3.50a | [https://www.baremetalsoft.com/baretail/](https://www.baremetalsoft.com/baretail/) |
| bat | 0.9.0 | [https://github.com/sharkdp/bat](https://github.com/sharkdp/bat) |
| bazel | 0.20.0 | [https://bazel.build](https://bazel.build) |
| beatdrop | 1.0.0.0 | [https://github.com/mvsoft74/BeatDrop](https://github.com/mvsoft74/BeatDrop) |
| beyondcompare | 4.2.8.23479 | [https://www.scootersoftware.com](https://www.scootersoftware.com) |
| bfg | 1.13.0 | [https://rtyley.github.io/bfg-repo-cleaner/](https://rtyley.github.io/bfg-repo-cleaner/) |
| bitmessage | 0.6.3.2 | [https://bitmessage.org/](https://bitmessage.org/) |
| bitwarden-cli | 1.6.0 | [https://bitwarden.com/](https://bitwarden.com/) |
| bitwarden | 1.11.2 | [https://bitwarden.com/](https://bitwarden.com/) |
| bleachbit | 2.0 | [https://www.bleachbit.org/](https://www.bleachbit.org/) |
| blender | 2.79b | [https://www.blender.org/](https://www.blender.org/) |
| blink1-tool | 2.0.2 | [https://blink1.thingm.com/](https://blink1.thingm.com/) |
| blink1control2 | 2.2.1 | [https://blink1.thingm.com/](https://blink1.thingm.com/) |
| blisk | 10.1.262.114 | [https://blisk.io/](https://blisk.io/) |
| bochs | 2.6.9 | [http://bochs.sourceforge.net/](http://bochs.sourceforge.net/) |
| boostnote | 0.11.11 | [https://boostnote.io/](https://boostnote.io/) |
| boot-clj | 2.7.2 | [https://github.com/boot-clj/boot](https://github.com/boot-clj/boot) |
| brackets | 1.13 | [http://brackets.io/](http://brackets.io/) |
| brave | 0.26.0 | [https://brave.com](https://brave.com) |
| brotli | 1.0.7 | [https://brotli.org/](https://brotli.org/) |
| buffalo | 0.13.10 | [https://gobuffalo.io](https://gobuffalo.io) |
| bulk-crap-uninstaller | 4.12.1 | [http://klocmansoftware.weebly.com/](http://klocmansoftware.weebly.com/) |
| busybox | 2358-g25a1bcec7 | [https://frippery.org/busybox](https://frippery.org/busybox) |
| bzip2 | 1.0.6 | [https://github.com/philr/bzip2-windows](https://github.com/philr/bzip2-windows) |
| cacert | 2018-12-05 | [https://curl.haxx.se/docs/caextract.html](https://curl.haxx.se/docs/caextract.html) |
| cacher | 2.2.0 | [https://www.cacher.io/](https://www.cacher.io/) |
| caddy | 0.11.1 | [https://caddyserver.com](https://caddyserver.com) |
| cake | 0.30.0 | [https://cakebuild.net/](https://cakebuild.net/) |
| calibre-normal | 3.35.0 | [https://calibre-ebook.com/](https://calibre-ebook.com/) |
| calibre | 3.35.0 | [https://calibre-ebook.com/](https://calibre-ebook.com/) |
| camunda-modeler | 2.2.3 | [https://camunda.org/download/modeler/](https://camunda.org/download/modeler/) |
| carnac | 2.2.155 | [http://carnackeys.com/](http://carnackeys.com/) |
| casperjs | 1.1.4-2 | [http://casperjs.org/](http://casperjs.org/) |
| ccat | 1.1.0 | [https://github.com/jingweno/ccat](https://github.com/jingweno/ccat) |
| ccleaner | 5.50.6911 | [https://www.piriform.com/ccleaner](https://www.piriform.com/ccleaner) |
| cdburnerxp | 4.5.8.7041 | [https://cdburnerxp.se/](https://cdburnerxp.se/) |
| cdrtools | 3.01 | [https://sourceforge.net/projects/tumagcc/](https://sourceforge.net/projects/tumagcc/) |
| championify | 2.1.5 | [https://github.com/dustinblackman/Championify](https://github.com/dustinblackman/Championify) |
| cheat-engine | 6.8.1 | [https://cheatengine.org/index.php](https://cheatengine.org/index.php) |
| chefdk | 3.5.13 | [https://chef.io](https://chef.io) |
| chrlauncher | 2.5.3 | [https://www.henrypp.org/product/chrlauncher](https://www.henrypp.org/product/chrlauncher) |
| chroma | 0.6.0 | [https://github.com/alecthomas/chroma](https://github.com/alecthomas/chroma) |
| chromedriver | 2.45 | [https://sites.google.com/a/chromium.org/chromedriver/](https://sites.google.com/a/chromium.org/chromedriver/) |
| chromium-dev-nosync | 68.0.3424.0-r556419 | [https://www.chromium.org](https://www.chromium.org) |
| chromium-dev | 72.0.3615.0-r609145 | [https://www.chromium.org](https://www.chromium.org) |
| chromium-nosync | 67.0.3396.99-r550428 | [https://www.chromium.org](https://www.chromium.org) |
| chromium | 71.0.3578.80-r599034 | [https://www.chromium.org](https://www.chromium.org) |
| clementine | 1.3.1 | [https://www.clementine-player.org/](https://www.clementine-player.org/) |
| clingo | 5.3.0 | [https://potassco.org/clingo/](https://potassco.org/clingo/) |
| clink | 0.4.9 | [https://mridgers.github.io/clink/](https://mridgers.github.io/clink/) |
| cloak | 0.1.0 | [https://github.com/evansmurithi/cloak](https://github.com/evansmurithi/cloak) |
| cloc | 1.70 | [https://github.com/AlDanial/cloc](https://github.com/AlDanial/cloc) |
| cloudfoundry-cli | 6.41.0 | [https://github.com/cloudfoundry/cli/](https://github.com/cloudfoundry/cli/) |
| cmake-rc | 3.13.0-rc3 | [https://cmake.org/](https://cmake.org/) |
| cmake | 3.13.1 | [https://cmake.org/](https://cmake.org/) |
| cmder-full | 1.3.10 | [http://cmder.net](http://cmder.net) |
| cmder | 1.3.10 | [http://cmder.net](http://cmder.net) |
| cmdow | 1.4.8 | [https://ritchielawrence.github.io/cmdow/](https://ritchielawrence.github.io/cmdow/) |
| cobalt | 0.14.0 | [https://cobalt-org.github.io/](https://cobalt-org.github.io/) |
| cockroachdb | 2.1.2 | [https://www.cockroachlabs.com/](https://www.cockroachlabs.com/) |
| codetrack | 1.0.3.3 | [http://www.getcodetrack.com](http://www.getcodetrack.com) |
| colortool | 1810.02002 | [https://github.com/Microsoft/Console/tree/master/tools/ColorTool](https://github.com/Microsoft/Console/tree/master/tools/ColorTool) |
| composer | 1.8.0 | [https://getcomposer.org/](https://getcomposer.org/) |
| concfg | 0.2018.10.22 | [https://github.com/lukesampson/concfg](https://github.com/lukesampson/concfg) |
| conemu | 18.06.26 | [https://conemu.github.io/](https://conemu.github.io/) |
| console2 | 2.0.0.148 | [https://sourceforge.net/projects/console/](https://sourceforge.net/projects/console/) |
| consolez | 1.18.3.18143 | [https://github.com/cbucher/console](https://github.com/cbucher/console) |
| consul | 1.4.0 | [https://www.consul.io](https://www.consul.io) |
| coretemp | 1.12.1 | [http://www.alcpu.com/CoreTemp/](http://www.alcpu.com/CoreTemp/) |
| coreutils | 5.97.3 | [http://www.mingw.org/wiki/msys](http://www.mingw.org/wiki/msys) |
| cowsay | 0.2013.07.19 | [https://github.com/lukesampson/cowsay-psh](https://github.com/lukesampson/cowsay-psh) |
| cppcheck | 1.86 | [http://cppcheck.sourceforge.net/](http://cppcheck.sourceforge.net/) |
| cpu-z | 1.87 | [https://www.cpuid.com/softwares/cpu-z.html](https://www.cpuid.com/softwares/cpu-z.html) |
| craft | april-2013 | [https://www.michaelfogleman.com/projects/craft/](https://www.michaelfogleman.com/projects/craft/) |
| crystaldiskinfo | 8.0.0 | [https://osdn.net/projects/crystaldiskinfo/](https://osdn.net/projects/crystaldiskinfo/) |
| crystaldiskmark | 6.0.2 | [https://osdn.net/projects/crystaldiskmark/](https://osdn.net/projects/crystaldiskmark/) |
| cscope | 15.8a | [http://cscope.sourceforge.net/](http://cscope.sourceforge.net/) |
| csvtosql | v0.1.1-alpha | [https://github.com/deevus/CsvToSql](https://github.com/deevus/CsvToSql) |
| ctags | 5.8 | [http://ctags.sourceforge.net/](http://ctags.sourceforge.net/) |
| cuetools | 2.1.6 | [http://cue.tools/wiki/Main_Page](http://cue.tools/wiki/Main_Page) |
| cura | 3.6.0 | [https://ultimaker.com/en/products/ultimaker-cura-software](https://ultimaker.com/en/products/ultimaker-cura-software) |
| curl | 7.63.0 | [https://curl.haxx.se/](https://curl.haxx.se/) |
| cutter | 1.7.2 | [https://github.com/radareorg/cutter](https://github.com/radareorg/cutter) |
| cygwin | 2.895 | [https://cygwin.com/](https://cygwin.com/) |
| darktable | 2.4.4 | [https://www.darktable.org/](https://www.darktable.org/) |
| dart-dev | 2.2.0-dev.0.0 | [https://www.dartlang.org/](https://www.dartlang.org/) |
| dart | 2.1.0 | [https://www.dartlang.org/](https://www.dartlang.org/) |
| darteditor | 1.6.0 | [https://www.dartlang.org](https://www.dartlang.org) |
| dartium-content-shell-dev | 1.25.0-dev.6.0 | [https://www.dartlang.org/](https://www.dartlang.org/) |
| dartium-content-shell | 1.24.2 | [https://www.dartlang.org/](https://www.dartlang.org/) |
| dartium-dev | 1.25.0-dev.6.0 | [https://www.dartlang.org/](https://www.dartlang.org/) |
| dartium | 1.24.2 | [https://www.dartlang.org/](https://www.dartlang.org/) |
| datamash | 1.3 | [https://www.gnu.org/software/datamash/](https://www.gnu.org/software/datamash/) |
| dbeaver | 5.3.0 | [https://dbeaver.io/](https://dbeaver.io/) |
| dbvis | 10.0.16 | [https://www.dbvis.com/](https://www.dbvis.com/) |
| dd | 0.6beta3 | [http://www.chrysocome.net/dd](http://www.chrysocome.net/dd) |
| ddev | 1.4.1 | [https://ddev.readthedocs.io/en/latest/](https://ddev.readthedocs.io/en/latest/) |
| ddu | 18.0.0.4 | [https://www.wagnardsoft.com/](https://www.wagnardsoft.com/) |
| deadlock | 1.4 | [https://codedead.com/](https://codedead.com/) |
| debugviewpp | 1.8.0.34 | [https://github.com/CobaltFusion/DebugViewPP](https://github.com/CobaltFusion/DebugViewPP) |
| defraggler | 2.22.995 | [https://www.ccleaner.com/defraggler](https://www.ccleaner.com/defraggler) |
| deluge | 1.3.15 | [http://deluge-torrent.org/](http://deluge-torrent.org/) |
| deno | 0.2.2 | [https://github.com/denoland/deno](https://github.com/denoland/deno) |
| dep | 0.5.0 | [https://github.com/golang/dep](https://github.com/golang/dep) |
| dependencies | 1.9 | [https://github.com/lucasg/Dependencies](https://github.com/lucasg/Dependencies) |
| depends | 2.2 | [http://www.dependencywalker.com/](http://www.dependencywalker.com/) |
| devd | 0.8 | [https://corte.si/posts/devd/intro/index.html](https://corte.si/posts/devd/intro/index.html) |
| devdocs | 0.6.9 | [https://github.com/egoist/devdocs-desktop](https://github.com/egoist/devdocs-desktop) |
| devrantron | 1.5.4 | [https://github.com/tahnik/devRantron](https://github.com/tahnik/devRantron) |
| dhcp-server | 2.5.2 | [http://www.dhcpserver.de](http://www.dhcpserver.de) |
| diff-pdf | 2012-02-28 | [http://vslavik.github.io/diff-pdf/](http://vslavik.github.io/diff-pdf/) |
| diffpdf | 2.1.3 | [http://soft.rubypdf.com/software/diffpdf](http://soft.rubypdf.com/software/diffpdf) |
| diffutils | 3.5 | [http://www.msys2.org](http://www.msys2.org) |
| dig | 9.13.4 | [https://www.isc.org/](https://www.isc.org/) |
| digdag | 0.9.31 | [https://www.digdag.io/](https://www.digdag.io/) |
| dirhash | 1.7.1 | [https://idrassi.github.io/DirHash](https://idrassi.github.io/DirHash) |
| discord-canary | 0.0.224 | [https://discordapp.com/](https://discordapp.com/) |
| discord-ptb | 0.0.43 | [https://discordapp.com/](https://discordapp.com/) |
| discord | 0.0.301 | [https://discordapp.com/](https://discordapp.com/) |
| dismplusplus | 10.1.1000.80 | [https://www.chuyu.me](https://www.chuyu.me) |
| ditto | 3.21.258.0 | [http://ditto-cp.sourceforge.net/](http://ditto-cp.sourceforge.net/) |
| dnsjumper | 2.1 | [https://www.sordum.org/dns-jumper/](https://www.sordum.org/dns-jumper/) |
| dnspy | 5.0.0 | [https://github.com/0xd4d/dnSpy](https://github.com/0xd4d/dnSpy) |
| docker-compose | 1.23.2 | [https://github.com/docker/compose](https://github.com/docker/compose) |
| docker-machine | 0.16.0 | [https://github.com/docker/machine](https://github.com/docker/machine) |
| docker-nightly | nightly | [https://master.dockerproject.org](https://master.dockerproject.org) |
| docker | 18.09.0 | [https://docker.com](https://docker.com) |
| dont-sleep | 4.91 | [https://www.softwareok.com/?Download=DontSleep](https://www.softwareok.com/?Download=DontSleep) |
| dopamine | 1.5.14 | [https://www.digimezzo.com/software/dopamine/](https://www.digimezzo.com/software/dopamine/) |
| dos2unix | 7.4.0 | [http://dos2unix.sourceforge.net/](http://dos2unix.sourceforge.net/) |
| dosbox | 0.74-2 | [https://www.dosbox.com/](https://www.dosbox.com/) |
| dotnet-sdk | 2.2.100 | [https://www.microsoft.com/net/](https://www.microsoft.com/net/) |
| dotnet | 1.1.1 | [https://www.microsoft.com/net/core#windows](https://www.microsoft.com/net/core#windows) |
| doublecmd | 0.8.4 | [https://doublecmd.sourceforge.io/](https://doublecmd.sourceforge.io/) |
| doxygen | 1.8.14 | [http://www.doxygen.nl/](http://www.doxygen.nl/) |
| draft | 0.16.0 | [https://github.com/Azure/draft](https://github.com/Azure/draft) |
| drone | 1.0.4 | [https://drone.io/](https://drone.io/) |
| ds4windows | 1.5.18 | [https://ryochan7.github.io/ds4windows-site/](https://ryochan7.github.io/ds4windows-site/) |
| duplicacy | 2.1.2 | [https://duplicacy.com/](https://duplicacy.com/) |
| eagleget-portable | 2.0.4.80 | [http://www.eagleget.com/](http://www.eagleget.com/) |
| easyrsa | 3.0.5 | [https://openvpn.net/easyrsa.html](https://openvpn.net/easyrsa.html) |
| easyserviceoptimizer | 1.2 | [https://www.sordum.org/files/easy-service-optimizer/](https://www.sordum.org/files/easy-service-optimizer/) |
| ec2-api-tools | 1.7.3.0 | [https://aws.amazon.com/developertools/351](https://aws.amazon.com/developertools/351) |
| echoargs | 3.2 | [https://pscx.codeplex.com/](https://pscx.codeplex.com/) |
| eclipse-android | 4.6.3 | [https://www.eclipse.org](https://www.eclipse.org) |
| eclipse-automotive | 4.5.2 | [https://www.eclipse.org](https://www.eclipse.org) |
| eclipse-committers | 2018-09 | [https://www.eclipse.org](https://www.eclipse.org) |
| eclipse-cpp | 2018-09 | [https://www.eclipse.org](https://www.eclipse.org) |
| eclipse-dsl | 2018-09 | [https://www.eclipse.org](https://www.eclipse.org) |
| eclipse-java | 2018-09 | [https://www.eclipse.org](https://www.eclipse.org) |
| eclipse-javascript | 2018-09 | [https://www.eclipse.org](https://www.eclipse.org) |
| eclipse-jee | 2018-09 | [https://www.eclipse.org](https://www.eclipse.org) |
| eclipse-mat | 1.8.1.20180910 | [https://www.eclipse.org/mat/](https://www.eclipse.org/mat/) |
| eclipse-modeling | 2018-09 | [https://www.eclipse.org](https://www.eclipse.org) |
| eclipse-parallel | 2018-09 | [https://www.eclipse.org](https://www.eclipse.org) |
| eclipse-php | 2018-09 | [https://www.eclipse.org](https://www.eclipse.org) |
| eclipse-platform | 4.9-201809060745 | [https://www.eclipse.org](https://www.eclipse.org) |
| eclipse-rcp | 2018-09 | [https://www.eclipse.org](https://www.eclipse.org) |
| eclipse-reporting | 2018-09 | [https://www.eclipse.org](https://www.eclipse.org) |
| eclipse-scout | 2018-09 | [https://www.eclipse.org](https://www.eclipse.org) |
| eclipse-sdk | 4.9-201809060745 | [https://www.eclipse.org](https://www.eclipse.org) |
| eclipse-testing | 2018-09 | [https://www.eclipse.org](https://www.eclipse.org) |
| edex-ui | 1.1.2 | [https://github.com/GitSquared/edex-ui](https://github.com/GitSquared/edex-ui) |
| edgedriver | 6.17134 | [https://developer.microsoft.com/en-us/microsoft-edge/tools/webdriver/#downloads](https://developer.microsoft.com/en-us/microsoft-edge/tools/webdriver/#downloads) |
| editorconfig | 0.12.1 | [http://editorconfig.org/](http://editorconfig.org/) |
| elasticsearch | 6.5.3 | [https://www.elastic.co/products/elasticsearch](https://www.elastic.co/products/elasticsearch) |
| elixir | 1.7.4 | [https://elixir-lang.org/](https://elixir-lang.org/) |
| elm | 0.19.0 | [http://elm-lang.org](http://elm-lang.org) |
| emacs | 26.1 | [https://www.gnu.org/software/emacs/](https://www.gnu.org/software/emacs/) |
| enpass | 5.6.10 | [https://www.enpass.io/](https://www.enpass.io/) |
| enso | 0.4.2 | [https://github.com/GChristensen/enso-portable](https://github.com/GChristensen/enso-portable) |
| erlang | 21.2 | [https://www.erlang.org](https://www.erlang.org) |
| etcher-cli | 1.4.8 | [https://etcher.io/cli](https://etcher.io/cli) |
| etcher | 1.4.8 | [https://etcher.io/](https://etcher.io/) |
| etlas | 1.5.0.0 | [https://github.com/typelead/etlas](https://github.com/typelead/etlas) |
| eventstore | 4.1.1-hotfix1 | [https://eventstore.org/](https://eventstore.org/) |
| everything | 1.4.1.895 | [https://www.voidtools.com/](https://www.voidtools.com/) |
| executor | 0.99.27b | [http://executor.dk/](http://executor.dk/) |
| exercism-cli | 3.0.11 | [http://exercism.io/](http://exercism.io/) |
| exercism | 3.0.11 | [https://github.com/exercism/cli](https://github.com/exercism/cli) |
| exiftool | 11.21 | [https://sno.phy.queensu.ca/~phil/exiftool/index.html](https://sno.phy.queensu.ca/~phil/exiftool/index.html) |
| faas-cli | 0.8.1 | [https://www.openfaas.com/](https://www.openfaas.com/) |
| falcon-sql-client | 4.0.0 | [https://plot.ly/free-sql-client-download](https://plot.ly/free-sql-client-download) |
| far | 30b5300 | [https://farmanager.com/](https://farmanager.com/) |
| fastcopy | 3.61 | [https://fastcopy.jp/en/](https://fastcopy.jp/en/) |
| fastglacier | 3.9.1 | [https://fastglacier.com](https://fastglacier.com) |
| fciv | 2.05 | [https://support.microsoft.com/en-us/kb/841290](https://support.microsoft.com/en-us/kb/841290) |
| fd | 7.2.0 | [https://github.com/sharkdp/fd](https://github.com/sharkdp/fd) |
| ffmpeg-nightly | 20181212-0e833f6 | [https://ffmpeg.zeranoe.com/builds/](https://ffmpeg.zeranoe.com/builds/) |
| ffmpeg | 4.1 | [https://ffmpeg.zeranoe.com/builds/](https://ffmpeg.zeranoe.com/builds/) |
| fiddler | 5.0.20182.28034 | [https://www.telerik.com/fiddler](https://www.telerik.com/fiddler) |
| figlet | 1.0-go | [https://github.com/lukesampson/figlet](https://github.com/lukesampson/figlet) |
| file | 5.03 | [http://gnuwin32.sourceforge.net/packages/file.htm](http://gnuwin32.sourceforge.net/packages/file.htm) |
| filezilla | 3.39.0 | [https://filezilla-project.org/](https://filezilla-project.org/) |
| find-java | 13 | [https://gist.github.com/se35710/43693e679701387d722206eff1e85f5f](https://gist.github.com/se35710/43693e679701387d722206eff1e85f5f) |
| findutils | 4.4.2 | [http://www.mingw.org/wiki/msys](http://www.mingw.org/wiki/msys) |
| firefox-beta | nightly | [https://www.mozilla.org/en-US/firefox/beta/](https://www.mozilla.org/en-US/firefox/beta/) |
| firefox-developer | nightly | [https://www.mozilla.org/en-US/firefox/developer/](https://www.mozilla.org/en-US/firefox/developer/) |
| firefox-esr | 60.4.0 | [https://www.mozilla.org/en-US/firefox/organizations/](https://www.mozilla.org/en-US/firefox/organizations/) |
| firefox-nightly | nightly | [https://www.mozilla.org/en-US/firefox/nightly/](https://www.mozilla.org/en-US/firefox/nightly/) |
| firefox | 64.0 | [https://www.mozilla.org/en-US/firefox/new/](https://www.mozilla.org/en-US/firefox/new/) |
| firewallappblocker | 1.6 | [https://www.sordum.org/files/firewall-app-blocker/](https://www.sordum.org/files/firewall-app-blocker/) |
| flatc | 1.10.0 | [https://google.github.io/flatbuffers/index.html](https://google.github.io/flatbuffers/index.html) |
| flow | 0.88.0 | [https://flowtype.org/](https://flowtype.org/) |
| flutter | 0.10.2 | [https://flutter.io/](https://flutter.io/) |
| flux | 4.84 | [https://justgetflux.com/](https://justgetflux.com/) |
| flyway | 5.2.4 | [https://flywaydb.org/](https://flywaydb.org/) |
| fmedia | 1.3 | [http://fmedia.firmdev.com/](http://fmedia.firmdev.com/) |
| fnproject | 0.5.35 | [https://fnproject.io/](https://fnproject.io/) |
| fnr | 1.8.1 | [https://github.com/zzzprojects/findandreplace](https://github.com/zzzprojects/findandreplace) |
| fontforge | 20170731-r2 | [https://fontforge.github.io](https://fontforge.github.io) |
| foobar2000-encoders | 2018-10-19 | [https://www.foobar2000.org/encoderpack](https://www.foobar2000.org/encoderpack) |
| foobar2000 | 1.4.1 | [https://www.foobar2000.org/](https://www.foobar2000.org/) |
| force | 0.25.0 | [https://force-cli.herokuapp.com/](https://force-cli.herokuapp.com/) |
| forego | 20180217041714 | [https://github.com/ddollar/forego](https://github.com/ddollar/forego) |
| forge | 2.2.0 | [http://forge.run](http://forge.run) |
| format-factory | 4.5.0.0 | [http://www.pcfreetime.com/formatfactory/index.php](http://www.pcfreetime.com/formatfactory/index.php) |
| fossil | 2.7 | [https://www.fossil-scm.org/](https://www.fossil-scm.org/) |
| foxe | 2.4.2 | [http://www.firstobject.com/dn_editor.htm](http://www.firstobject.com/dn_editor.htm) |
| foxit-reader | 9.3.0.10826 | [https://www.foxitsoftware.com/](https://www.foxitsoftware.com/) |
| franz | 5.0.0-beta.19 | [http://meetfranz.com](http://meetfranz.com) |
| freac | 1.0.32 | [https://www.freac.org](https://www.freac.org) |
| freeclipboardviewer | 3.0 | [http://www.freeclipboardviewer.com/](http://www.freeclipboardviewer.com/) |
| freecommander | 2018 | [https://freecommander.com](https://freecommander.com) |
| freemind | 1.0.1 | [http://freemind.sourceforge.net/wiki/index.php/Main_Page](http://freemind.sourceforge.net/wiki/index.php/Main_Page) |
| fscapture | 5.3 | [http://www.faststone.org/FSCaptureDetail.htm](http://www.faststone.org/FSCaptureDetail.htm) |
| fsviewer | 6.7 | [http://www.faststone.org/FSViewerDetail.htm](http://www.faststone.org/FSViewerDetail.htm) |
| fzf | 0.17.5 | [https://github.com/junegunn/fzf](https://github.com/junegunn/fzf) |
| gawk | 3.1.7 | [http://www.mingw.org/wiki/MSYS](http://www.mingw.org/wiki/MSYS) |
| gcc-arm-none-eabi | 7-2018-q2-update | [https://developer.arm.com/open-source/gnu-toolchain/gnu-rm](https://developer.arm.com/open-source/gnu-toolchain/gnu-rm) |
| gcc | 8.1.0 | [https://mingw-w64.org](https://mingw-w64.org) |
| gcloud | 228.0.0 | [https://cloud.google.com/sdk/](https://cloud.google.com/sdk/) |
| gdb | 7.9.1 | [http://tdm-gcc.tdragon.net/](http://tdm-gcc.tdragon.net/) |
| geany | 1.33 | [https://www.geany.org/](https://www.geany.org/) |
| geckodriver | 0.23.0 | [https://github.com/mozilla/geckodriver](https://github.com/mozilla/geckodriver) |
| geekuninstaller | 1.4.5.134 | [https://geekuninstaller.com/](https://geekuninstaller.com/) |
| genact | 0.6.0 | [https://github.com/svenstaro/genact/](https://github.com/svenstaro/genact/) |
| ghostscript | 9.26 | [https://www.ghostscript.com](https://www.ghostscript.com) |
| ghostwriter | 1.7.1 | [https://wereturtle.github.io/ghostwriter/](https://wereturtle.github.io/ghostwriter/) |
| ghq | 0.8.0 | [https://github.com/motemen/ghq](https://github.com/motemen/ghq) |
| gibo | 2.1.0 | [https://github.com/simonwhitaker/gibo](https://github.com/simonwhitaker/gibo) |
| gifcam | 5.5 | [http://blog.bahraniapps.com/gifcam/](http://blog.bahraniapps.com/gifcam/) |
| gifsicle | 1.89 | [http://www.lcdf.org/gifsicle/](http://www.lcdf.org/gifsicle/) |
| gimp | 2.10.8 | [https://www.gimp.org/](https://www.gimp.org/) |
| git-annex | 7.20181211 | [http://git-annex.branchable.com/](http://git-annex.branchable.com/) |
| git-crypt | 0.6.0-701fb8e | [https://www.agwa.name/projects/git-crypt/](https://www.agwa.name/projects/git-crypt/) |
| git-istage | 0.2.61 | [https://github.com/terrajobst/git-istage](https://github.com/terrajobst/git-istage) |
| git-lfs | 2.6.1 | [https://git-lfs.github.com/](https://git-lfs.github.com/) |
| git-sizer | 1.3.0 | [https://github.com/github/git-sizer](https://github.com/github/git-sizer) |
| git-town | 7.2.0 | [http://www.git-town.com/](http://www.git-town.com/) |
| git-up | 1.6.0 | [https://github.com/msiemens/PyGitUp](https://github.com/msiemens/PyGitUp) |
| git-with-openssh | 2.20.0.windows.1 | [https://git-for-windows.github.io/](https://git-for-windows.github.io/) |
| git | 2.20.0.windows.1 | [https://git-for-windows.github.io/](https://git-for-windows.github.io/) |
| git19 | 1.9.5-preview20150319 | [https://git-for-windows.github.io/](https://git-for-windows.github.io/) |
| gitea | 1.6.1 | [https://gitea.io/](https://gitea.io/) |
| gitextensions | 2.51.05 | [https://gitextensions.github.io/](https://gitextensions.github.io/) |
| github | 1.5.0 | [https://desktop.github.com/](https://desktop.github.com/) |
| gitignore | 0.2018.08.04 | [https://github.com/lukesampson/psutils](https://github.com/lukesampson/psutils) |
| gitkraken | 4.1.1 | [https://www.gitkraken.com/](https://www.gitkraken.com/) |
| gitlab-runner | 11.5.1 | [https://docs.gitlab.com/runner/](https://docs.gitlab.com/runner/) |
| gitversion | 4.0.0 | [https://gitversion.readthedocs.io/](https://gitversion.readthedocs.io/) |
| glide | 0.13.2 | [https://glide.sh/](https://glide.sh/) |
| glogg | 1.1.4 | [https://glogg.bonnefon.org/](https://glogg.bonnefon.org/) |
| glslang-nightly | nightly | [https://www.khronos.org/opengles/sdk/tools/Reference-Compiler/](https://www.khronos.org/opengles/sdk/tools/Reference-Compiler/) |
| glslang | 7.10.2984 | [https://www.khronos.org/opengles/sdk/tools/Reference-Compiler/](https://www.khronos.org/opengles/sdk/tools/Reference-Compiler/) |
| gnirehtet | 2.3 | [https://github.com/Genymobile/gnirehtet](https://github.com/Genymobile/gnirehtet) |
| gnucash | 3.2 | [https://www.gnucash.org/](https://www.gnucash.org/) |
| gnupg | 2.2.11 | [https://www.gnupg.org/](https://www.gnupg.org/) |
| gnupg1 | 1.4.23 | [https://www.gnupg.org/](https://www.gnupg.org/) |
| go-ipfs | 0.4.18 | [https://ipfs.io/](https://ipfs.io/) |
| go | 1.11.2 | [https://golang.org](https://golang.org) |
| godot-mono | 3.0.6 | [https://godotengine.org/](https://godotengine.org/) |
| godot | 3.0.6 | [https://godotengine.org/](https://godotengine.org/) |
| gof | 0.0.1 | [https://github.com/mattn/gof](https://github.com/mattn/gof) |
| gogs | 0.11.79 | [https://gogs.io/](https://gogs.io/) |
| goldendict | 1.5.0-RC2-311-g15062f7 | [https://sourceforge.net/projects/goldendict/](https://sourceforge.net/projects/goldendict/) |
| google-java-format | 1.6 | [https://github.com/google/google-java-format](https://github.com/google/google-java-format) |
| gopass | 1.8.3 | [https://www.gopass.pw/](https://www.gopass.pw/) |
| gource | 0.47 | [http://gource.io/](http://gource.io/) |
| gow | 0.8.0 | [https://github.com/bmatzelle/gow](https://github.com/bmatzelle/gow) |
| gpg | 2.2.11 | [https://www.gnupg.org/](https://www.gnupg.org/) |
| gpg4win | 3.1.5 | [https://www.gpg4win.org](https://www.gpg4win.org) |
| gpu-z | 2.16.0 | [https://www.techpowerup.com/gpuz/](https://www.techpowerup.com/gpuz/) |
| gradle-bin | 5.0 | [https://gradle.org](https://gradle.org) |
| gradle | 5.0 | [https://gradle.org](https://gradle.org) |
| grafana | 5.4.1 | [https://grafana.com/](https://grafana.com/) |
| grails | 3.3.9 | [https://grails.org/](https://grails.org/) |
| graphicsgale | 2.08.19 | [https://graphicsgale.com/us/](https://graphicsgale.com/us/) |
| graphicsmagick-q16 | 1.3.31 | [http://www.graphicsmagick.org/](http://www.graphicsmagick.org/) |
| graphicsmagick-q8 | 1.3.31 | [http://www.graphicsmagick.org/](http://www.graphicsmagick.org/) |
| graphviz | 2.38 | [https://www.graphviz.org/](https://www.graphviz.org/) |
| greenshot | 1.2.10.6 | [https://getgreenshot.org](https://getgreenshot.org) |
| grep | 2.5.4 | [http://gnuwin32.sourceforge.net/packages/grep.htm](http://gnuwin32.sourceforge.net/packages/grep.htm) |
| groovy | 2.5.4 | [http://www.groovy-lang.org/](http://www.groovy-lang.org/) |
| groovyserv | 1.2.0 | [https://kobo.github.io/groovyserv/](https://kobo.github.io/groovyserv/) |
| guetzli | 1.0.1 | [https://github.com/google/guetzli](https://github.com/google/guetzli) |
| gzip | 1.3.12 | [http://www.mingw.org/wiki/msys](http://www.mingw.org/wiki/msys) |
| hack-font | 1.6.0 | [https://sourcefoundry.org/hack/](https://sourcefoundry.org/hack/) |
| hadoop-winutils | 2.8.1 | [https://github.com/steveloughran/winutils](https://github.com/steveloughran/winutils) |
| hain | 0.6.6 | [http://hainproject.github.io/hain/](http://hainproject.github.io/hain/) |
| HamMultiPlayer | 0.116.37905.792 | [http://hammultiplayer.org](http://hammultiplayer.org) |
| handbrake-cli | 1.1.2 | [https://handbrake.fr/](https://handbrake.fr/) |
| handbrake | 1.1.2 | [https://handbrake.fr/](https://handbrake.fr/) |
| harmony | 0.9.1 | [https://getharmony.xyz/](https://getharmony.xyz/) |
| hashcat | 5.1.0 | [https://hashcat.net/hashcat/](https://hashcat.net/hashcat/) |
| haskell | 8.4.3 | [https://www.haskell.org](https://www.haskell.org) |
| haskellx | 7.8.3 | [https://www.haskell.org](https://www.haskell.org) |
| haxe | 3.4.7 | [https://haxe.org/](https://haxe.org/) |
| heidisql | 9.5 | [https://www.heidisql.com/](https://www.heidisql.com/) |
| helm | 2.12.0 | [https://helm.sh/](https://helm.sh/) |
| helmfile | 0.40.3 | [https://github.com/roboll/helmfile/](https://github.com/roboll/helmfile/) |
| heroku-cli | nightly | []() |
| hexchat | 2.14.2 | [https://hexchat.github.io](https://hexchat.github.io) |
| highlight | 3.47 | [http://www.andre-simon.de/doku/highlight/en/highlight.php](http://www.andre-simon.de/doku/highlight/en/highlight.php) |
| honeyview | 5.31 | [https://www.bandisoft.com/honeyview/](https://www.bandisoft.com/honeyview/) |
| hostsman | 4.7.105 | [http://www.abelhadigital.com/hostsman](http://www.abelhadigital.com/hostsman) |
| httrack | 3.49.2 | [https://www.httrack.com/](https://www.httrack.com/) |
| hub | 2.6.1 | [https://hub.github.com/](https://hub.github.com/) |
| hugo | 0.52 | [https://gohugo.io](https://gohugo.io) |
| hwinfo | 5.92-3580 | [https://www.hwinfo.com/](https://www.hwinfo.com/) |
| hwmonitor | 1.38 | [https://www.cpuid.com/softwares/hwmonitor.html](https://www.cpuid.com/softwares/hwmonitor.html) |
| hxd | 2.1.0.0 | [https://mh-nexus.de/en/hxd/](https://mh-nexus.de/en/hxd/) |
| hygen | 1.6.4 | [https://www.hygen.io/](https://www.hygen.io/) |
| hyper | 2.0.0 | [https://hyper.is](https://hyper.is) |
| hyperfine | 1.4.0 | [https://github.com/sharkdp/hyperfine](https://github.com/sharkdp/hyperfine) |
| ibmcloud-cli | 0.12.1 | [https://github.com/IBM-Bluemix/bluemix-cli-release](https://github.com/IBM-Bluemix/bluemix-cli-release) |
| iconv | 1.14-3 | [http://www.mingw.org/](http://www.mingw.org/) |
| idea-eap | 183.4139.22 | [https://www.jetbrains.com/idea/](https://www.jetbrains.com/idea/) |
| idea-ultimate-eap | 183.4139.22 | [https://www.jetbrains.com/idea/](https://www.jetbrains.com/idea/) |
| idea-ultimate | 2018.3.1 | [https://www.jetbrains.com/idea/](https://www.jetbrains.com/idea/) |
| idea | 2018.3.1 | [https://www.jetbrains.com/idea/](https://www.jetbrains.com/idea/) |
| idris | 1.3.1 | [https://www.idris-lang.org/](https://www.idris-lang.org/) |
| ie11webdriver | 3.14.0 | [http://www.seleniumhq.org/](http://www.seleniumhq.org/) |
| ilspy | 3.2.0.3856 | [http://ilspy.net/](http://ilspy.net/) |
| imageglass | 5.5.7.26 | [http://www.imageglass.org/](http://www.imageglass.org/) |
| imagemagick | 7.0.8-16 | [https://www.imagemagick.org/script/index.php](https://www.imagemagick.org/script/index.php) |
| imgburn | 2.5.8.0 | [http://www.imgburn.com/](http://www.imgburn.com/) |
| inadyn-mt | 02.28.10 | [https://sourceforge.net/projects/inadyn-mt/files/inadyn-mt/](https://sourceforge.net/projects/inadyn-mt/files/inadyn-mt/) |
| inboxer | 1.2.1 | [https://denysdovhan.com/inboxer/](https://denysdovhan.com/inboxer/) |
| influxdb | 1.7.1 | [https://www.influxdata.com/](https://www.influxdata.com/) |
| inkscape | 0.92.3 | [https://inkscape.org/](https://inkscape.org/) |
| inkscape32bit | 0.92.3 | [https://inkscape.org/](https://inkscape.org/) |
| innoextract | 1.7 | [http://constexpr.org/innoextract/](http://constexpr.org/innoextract/) |
| innounp | 0.47 | [http://innounp.sourceforge.net](http://innounp.sourceforge.net) |
| insect | 5.0.0 | [https://github.com/sharkdp/insect](https://github.com/sharkdp/insect) |
| insomnia | 6.2.3 | [https://insomnia.rest](https://insomnia.rest) |
| invoke-build | 5.4.2 | [https://github.com/nightroman/Invoke-Build](https://github.com/nightroman/Invoke-Build) |
| iographica | 1.0.1 | [http://www.iographica.com/](http://www.iographica.com/) |
| ios-webkit-debug-proxy | 1.8.3 | [https://github.com/google/ios-webkit-debug-proxy](https://github.com/google/ios-webkit-debug-proxy) |
| iperf3 | 3.1.3 | [https://iperf.fr/](https://iperf.fr/) |
| ipfilter-updater | 3.0.0 | [https://www.sadrobot.co.nz/ipfilter/](https://www.sadrobot.co.nz/ipfilter/) |
| ipscan | 3.5.3 | [http://angryip.org/](http://angryip.org/) |
| irfanview | 4.51 | [https://www.irfanview.com/](https://www.irfanview.com/) |
| jameica | 2.8.2 | [https://www.willuhn.de/products/jameica/](https://www.willuhn.de/products/jameica/) |
| jd-cmd | 0.9.2 | [https://github.com/kwart/jd-cmd](https://github.com/kwart/jd-cmd) |
| jd-gui | 1.4.0 | [http://jd.benow.ca/](http://jd.benow.ca/) |
| jdownloader | nightly | [http://jdownloader.org/](http://jdownloader.org/) |
| jetbrains-toolbox | 1.12.4481 | [https://jetbrains.com/](https://jetbrains.com/) |
| jfrog | 1.22.1 | [https://jfrog.com/getcli/](https://jfrog.com/getcli/) |
| jhead | 3.00 | [http://www.sentex.net/~mwandel/jhead/](http://www.sentex.net/~mwandel/jhead/) |
| jigsaw | 2.2.6 | [https://www.w3.org/Jigsaw](https://www.w3.org/Jigsaw) |
| jira | 1.0.20 | [https://github.com/Netflix-Skunkworks/go-jira](https://github.com/Netflix-Skunkworks/go-jira) |
| jitsi-meet-electron | 1.1.1 | [https://github.com/jitsi/jitsi-meet-electron](https://github.com/jitsi/jitsi-meet-electron) |
| jkrypto | 4.4 | [http://lpb.canb.auug.org.au/adfa/src/jkrypto/index.html](http://lpb.canb.auug.org.au/adfa/src/jkrypto/index.html) |
| joe | 4.6 | [https://joe-editor.sourceforge.io/](https://joe-editor.sourceforge.io/) |
| joplin | 1.0.117 | [https://joplin.cozic.net/](https://joplin.cozic.net/) |
| jpegview | 1.0.37 | [https://downloads.sourceforge.net/project/jpegview/](https://downloads.sourceforge.net/project/jpegview/) |
| jq | 1.6 | [https://stedolan.github.io/jq/](https://stedolan.github.io/jq/) |
| jruby | 9.2.5.0 | [https://www.jruby.org/](https://www.jruby.org/) |
| julia | 1.0.2 | [https://julialang.org](https://julialang.org) |
| just | 0.3.13 | [https://github.com/casey/just](https://github.com/casey/just) |
| kakaotalk | 2.7.0.1858 | [https://www.kakao.com/talk](https://www.kakao.com/talk) |
| kdenlive | 18.08.2 | [https://kdenlive.org/](https://kdenlive.org/) |
| kdiff3 | 0.9.98 | [http://kdiff3.sourceforge.net/](http://kdiff3.sourceforge.net/) |
| keepass | 2.40 | [https://keepass.info/](https://keepass.info/) |
| keepassxc | 2.3.4 | [https://keepassxc.org/](https://keepassxc.org/) |
| keeweb | 1.6.3 | [https://keeweb.info/](https://keeweb.info/) |
| keypirinha | 2.23 | [http://keypirinha.com](http://keypirinha.com) |
| keystore-explorer | 5.4.1 | [https://keystore-explorer.org/](https://keystore-explorer.org/) |
| kibana | 6.5.3 | [https://www.elastic.co/products/kibana](https://www.elastic.co/products/kibana) |
| kicad | 5.0.2_1 | [http://kicad-pcb.org/](http://kicad-pcb.org/) |
| kid3 | 3.6.2 | [https://kid3.sourceforge.io](https://kid3.sourceforge.io) |
| kindlegen | 2.9 | [https://www.amazon.com/gp/feature.html?docId=1000765211](https://www.amazon.com/gp/feature.html?docId=1000765211) |
| kitematic | 0.17.6 | [https://github.com/docker/kitematic](https://github.com/docker/kitematic) |
| kitty | 0.70.0.7 | [http://kitty.9bis.net](http://kitty.9bis.net) |
| knime | 3.7.0 | [https://www.knime.com/](https://www.knime.com/) |
| kompose | 1.17.0 | [http://kompose.io](http://kompose.io) |
| kotlin-native | 0.9.3 | [https://kotlinlang.org/](https://kotlinlang.org/) |
| kotlin | 1.3.11 | [https://kotlinlang.org/](https://kotlinlang.org/) |
| krita | 4.1.5 | [https://krita.org/](https://krita.org/) |
| ktlint | 0.29.0 | [https://github.com/shyiko/ktlint](https://github.com/shyiko/ktlint) |
| kubectl | 1.13.0 | [https://kubernetes.io/docs/user-guide/kubectl-overview/](https://kubernetes.io/docs/user-guide/kubectl-overview/) |
| lame | 3.100 | [https://lame.sourceforge.net/](https://lame.sourceforge.net/) |
| latex | 2.9.6753 | [https://miktex.org](https://miktex.org) |
| launchy | 2.9.57 | [https://openningia.github.io/Launchy](https://openningia.github.io/Launchy) |
| lazygit | 0.5 | [https://github.com/jesseduffield/lazygit](https://github.com/jesseduffield/lazygit) |
| lcow | v4.14.35-v0.3.9 | [https://github.com/linuxkit/lcow](https://github.com/linuxkit/lcow) |
| ldap-admin | 1.8.3 | [http://ldapadmin.org/](http://ldapadmin.org/) |
| ldc | 1.12.0 | [https://dlang.org/](https://dlang.org/) |
| leet | 2014.8.29 | [https://github.com/vidarkongsli/posh1337](https://github.com/vidarkongsli/posh1337) |
| leiningen | 2.8.2 | [https://github.com/technomancy/leiningen](https://github.com/technomancy/leiningen) |
| less | 530 | [http://www.greenwoodsoftware.com/less/](http://www.greenwoodsoftware.com/less/) |
| lessmsi | 1.6.3 | [https://github.com/activescott/lessmsi/](https://github.com/activescott/lessmsi/) |
| lf | r8 | [https://godoc.org/github.com/gokcehan/lf](https://godoc.org/github.com/gokcehan/lf) |
| libreoffice-fresh | 6.1.3.2 | [https://libreoffice.org/](https://libreoffice.org/) |
| libsndfile | 1.0.28 | [http://www.mega-nerd.com/libsndfile/](http://www.mega-nerd.com/libsndfile/) |
| libwebp | 1.0.0 | [https://developers.google.com/speed/webp/](https://developers.google.com/speed/webp/) |
| licecap | 1.26 | [https://www.cockos.com/licecap/](https://www.cockos.com/licecap/) |
| lightbulb | 1.6.4.1 | [https://github.com/Tyrrrz/LightBulb](https://github.com/Tyrrrz/LightBulb) |
| lightshot | nightly | [https://prnt.sc](https://prnt.sc) |
| lighttable | 0.8.1 | [http://www.lighttable.com/](http://www.lighttable.com/) |
| lighttpd | 1.4.49-1 | [http://lighttpd.dtech.hu/](http://lighttpd.dtech.hu/) |
| lili | 2.9.4 | [https://www.linuxliveusb.com](https://www.linuxliveusb.com) |
| lilypond | 2.18.2 | [http://lilypond.org](http://lilypond.org) |
| linqpad | nightly | [https://www.linqpad.net](https://www.linqpad.net) |
| linqpadless | 1.1.0 | [https://github.com/linqpadless/LinqPadless](https://github.com/linqpadless/LinqPadless) |
| listenmoeclient | 2.0.0 | [https://github.com/LISTEN-moe/windows-app](https://github.com/LISTEN-moe/windows-app) |
| llvm | 7.0.0 | [https://www.llvm.org/](https://www.llvm.org/) |
| lmms | 1.1.3 | [https://lmms.io/](https://lmms.io/) |
| ln | 0.2018.08.04 | [https://github.com/lukesampson/psutils](https://github.com/lukesampson/psutils) |
| lockhunter | 3.2.3 | [https://lockhunter.com/index.htm](https://lockhunter.com/index.htm) |
| logexpert | 1.6.13 | [https://github.com/zarunbal/LogExpert](https://github.com/zarunbal/LogExpert) |
| logstash | 5.6.1 | [https://www.elastic.co/products/logstash](https://www.elastic.co/products/logstash) |
| losslesscut | 1.14.0 | [https://github.com/mifi/lossless-cut](https://github.com/mifi/lossless-cut) |
| love | 11.2 | [https://love2d.org/](https://love2d.org/) |
| lua | 5.1.5-52 | [https://github.com/rjpcomputing/luaforwindows](https://github.com/rjpcomputing/luaforwindows) |
| lunacy | 3.12 | [https://icons8.com/lunacy](https://icons8.com/lunacy) |
| lxrunoffline | 3.3.2 | [https://github.com/DDoSolitary/LxRunOffline](https://github.com/DDoSolitary/LxRunOffline) |
| lynx | 2.8.9rel.1 | [http://invisible-island.net/lynx/lynx.html](http://invisible-island.net/lynx/lynx.html) |
| lzip | 1.20 | [https://www.nongnu.org/lzip/lzip.html](https://www.nongnu.org/lzip/lzip.html) |
| madvr | 0.92.17 | [http://madvr.com/](http://madvr.com/) |
| mailsend | 1.19 | [https://github.com/muquit/mailsend](https://github.com/muquit/mailsend) |
| make | 4.2 | [https://www.gnu.org/software/make/](https://www.gnu.org/software/make/) |
| makemkv | 1.14.2 | [https://www.makemkv.com/](https://www.makemkv.com/) |
| mancy | 3.2.0 | [http://mancy-re.pl/](http://mancy-re.pl/) |
| mariadb | 10.3.11 | [https://mariadb.org](https://mariadb.org) |
| maven | 3.6.0 | [https://maven.apache.org/](https://maven.apache.org/) |
| mc | 4.8.19 | [https://midnight-commander.org/](https://midnight-commander.org/) |
| MediaCreationTool | 10.0.17763.1 | [https://www.microsoft.com/en-us/software-download/windows10](https://www.microsoft.com/en-us/software-download/windows10) |
| mediainfo-gui | 18.12 | [https://mediaarea.net/en/MediaInfo](https://mediaarea.net/en/MediaInfo) |
| mediainfo | 18.12 | [https://mediaarea.net/en/MediaInfo](https://mediaarea.net/en/MediaInfo) |
| megasync | 3.7.1.0 | [https://mega.nz/](https://mega.nz/) |
| meld | 3.18.3 | [http://meldmerge.org/](http://meldmerge.org/) |
| mercurial | 4.8.1 | [https://www.mercurial-scm.org/](https://www.mercurial-scm.org/) |
| metastore | 1.1.2-9-gdafa727 | [https://github.com/rasa/metastore](https://github.com/rasa/metastore) |
| micro | 1.4.1 | [https://micro-editor.github.io/](https://micro-editor.github.io/) |
| microsip | 3.19.8 | [https://www.microsip.org](https://www.microsip.org) |
| mill | 0.3.5 | [http://www.lihaoyi.com/mill/](http://www.lihaoyi.com/mill/) |
| mingit-busybox | 2.20.0.windows.1 | [https://git-for-windows.github.io/](https://git-for-windows.github.io/) |
| mingit | 2.20.0.windows.1 | [https://git-for-windows.github.io/](https://git-for-windows.github.io/) |
| miniconda3 | 4.5.11 | [https://conda.io/miniconda.html](https://conda.io/miniconda.html) |
| minikube | 0.31.0 | [https://kubernetes.io/docs/getting-started-guides/minikube/](https://kubernetes.io/docs/getting-started-guides/minikube/) |
| minio-client | 2018-12-05T22-59-07Z | [https://minio.io/](https://minio.io/) |
| minio | 2018-12-06T01-27-43Z | [https://minio.io/](https://minio.io/) |
| minishift | 1.28.0 | [https://www.openshift.org/minishift](https://www.openshift.org/minishift) |
| minisign | 0.8 | [https://jedisct1.github.io/minisign/](https://jedisct1.github.io/minisign/) |
| mitmproxy | 4.0.4 | [https://mitmproxy.org/](https://mitmproxy.org/) |
| mkcert | 1.1.2 | [https://github.com/FiloSottile/mkcert](https://github.com/FiloSottile/mkcert) |
| mkvtoolnix | 29.0.0 | [https://mkvtoolnix.download/](https://mkvtoolnix.download/) |
| mls-software-openssh | 7.9p1-1 | [https://www.mls-software.com/opensshd.html](https://www.mls-software.com/opensshd.html) |
| mobaxterm | 11.0 | [https://mobaxterm.mobatek.net/](https://mobaxterm.mobatek.net/) |
| modd | 0.7 | [https://corte.si/posts/modd/announce/index.html](https://corte.si/posts/modd/announce/index.html) |
| monero | 0.13.0.4 | [https://getmonero.org/](https://getmonero.org/) |
| mongodb-compass-community | 1.16.3 | [https://www.mongodb.com/download-center?jmp=hero#compass](https://www.mongodb.com/download-center?jmp=hero#compass) |
| mongodb | 4.0.4 | [https://www.mongodb.org](https://www.mongodb.org) |
| mono | 5.16.0.220 | [http://www.mono-project.com/](http://www.mono-project.com/) |
| moonscript | 0.5.0 | [https://moonscript.org/](https://moonscript.org/) |
| mousejiggler | 1.7.4 | [https://github.com/cerebrate/mousejiggler](https://github.com/cerebrate/mousejiggler) |
| mozjpeg | 3.3.1 | [https://github.com/mozilla/mozjpeg](https://github.com/mozilla/mozjpeg) |
| mp3tag | 2.91 | [https://www.mp3tag.de/](https://www.mp3tag.de/) |
| mpc-be | 1.5.2 | [https://sourceforge.net/projects/mpcbe/](https://sourceforge.net/projects/mpcbe/) |
| mpc-hc-fork | 1.8.3 | [https://github.com/clsid2/mpc-hc](https://github.com/clsid2/mpc-hc) |
| mpc-hc | 1.7.13 | [https://mpc-hc.org/](https://mpc-hc.org/) |
| mpc-qt | 18.08 | [https://github.com/cmdrkotori/mpc-qt](https://github.com/cmdrkotori/mpc-qt) |
| mplayer | 38117 | [http://mplayerwin.sourceforge.net/](http://mplayerwin.sourceforge.net/) |
| mpv-git | 20181202 | [https://mpv.io/](https://mpv.io/) |
| mpv | 2018-10-02 | [https://mpv.io/](https://mpv.io/) |
| mqtt-spy | 1.0.0 | [https://github.com/eclipse/paho.mqtt-spy](https://github.com/eclipse/paho.mqtt-spy) |
| mremoteng | 1.76.11.40527 | [https://mremoteng.org/](https://mremoteng.org/) |
| msiafterburner | 4.5.0 | [https://www.msi.com/page/afterburner](https://www.msi.com/page/afterburner) |
| msmpi | 9.0.1 | [https://www.microsoft.com/en-us/download/details.aspx?id=56727](https://www.microsoft.com/en-us/download/details.aspx?id=56727) |
| msys | rev13 | []() |
| msys2 | 20180531 | [http://msys2.github.io](http://msys2.github.io) |
| mupdf | 1.14.0 | [https://mupdf.com/](https://mupdf.com/) |
| musescore | 2.3.2 | [https://musescore.org/](https://musescore.org/) |
| musicbee | 3.2.6827 | [https://getmusicbee.com/](https://getmusicbee.com/) |
| mysql-workbench | 8.0.13 | [https://dev.mysql.com/downloads/workbench/](https://dev.mysql.com/downloads/workbench/) |
| mysql | 8.0.13 | [https://dev.mysql.com/downloads/mysql/](https://dev.mysql.com/downloads/mysql/) |
| nano | 2.5.3 | [https://www.nano-editor.org/](https://www.nano-editor.org/) |
| naps2 | 5.8.2 | [https://www.naps2.com/](https://www.naps2.com/) |
| nasm | 2.14 | [http://www.nasm.us](http://www.nasm.us) |
| natural-docs | 2.0.2 | [http://www.naturaldocs.org/](http://www.naturaldocs.org/) |
| ncftpclient | 3.2.6 | [https://www.ncftp.com/](https://www.ncftp.com/) |
| neko | 2.2.0 | [https://nekovm.org/](https://nekovm.org/) |
| neofetch | 5.0.0 | [https://github.com/dylanaraps/neofetch](https://github.com/dylanaraps/neofetch) |
| neovim | 0.3.1 | [https://neovim.io/](https://neovim.io/) |
| netbeans | 9.0 | [https://netbeans.org](https://netbeans.org) |
| netcat | 1.12 | [https://eternallybored.org/misc/netcat/](https://eternallybored.org/misc/netcat/) |
| netlifyctl | 0.4.0 | [https://www.netlify.com/](https://www.netlify.com/) |
| nexusfont | 2.6.2.1870 | [http://www.xiles.net/](http://www.xiles.net/) |
| nginx | 1.15.7 | [https://nginx.org](https://nginx.org) |
| ngrok | 4VmDzA7iaHb | [https://ngrok.com/](https://ngrok.com/) |
| nikto | 2.1.5 | [https://projects.giacomodrago.com/nikto-win/](https://projects.giacomodrago.com/nikto-win/) |
| nim | 0.19.0 | [https://nim-lang.org/](https://nim-lang.org/) |
| nimbleset | 2.2.0.41590 | [http://nimbletext.com/SET/About](http://nimbletext.com/SET/About) |
| nimbletext | 2.9.1.36018 | [http://nimbletext.com/](http://nimbletext.com/) |
| ninja | 1.8.2 | [https://ninja-build.org/](https://ninja-build.org/) |
| nircmd | 2.81 | [https://www.nirsoft.net/utils/nircmd.html](https://www.nirsoft.net/utils/nircmd.html) |
| nirlauncher | 1.20.64 | [https://launcher.nirsoft.net/](https://launcher.nirsoft.net/) |
| nmap | 7.70 | [https://nmap.org](https://nmap.org) |
| node-chakracore | 10.13.0 | [https://github.com/nodejs/node-chakracore](https://github.com/nodejs/node-chakracore) |
| node-compiler | 1.5.0 | [https://github.com/lastmjs/node-compiler](https://github.com/lastmjs/node-compiler) |
| nodejs-lts | 10.14.2 | [https://nodejs.org](https://nodejs.org) |
| nodejs | 11.4.0 | [https://nodejs.org](https://nodejs.org) |
| nomacs | 3.12.1 | [https://nomacs.org](https://nomacs.org) |
| notepad2-mod | 4.2.25.998 | [https://github.com/XhmikosR/notepad2-mod](https://github.com/XhmikosR/notepad2-mod) |
| notepad2 | 4.2.25 | [http://www.flos-freeware.ch/notepad2.html](http://www.flos-freeware.ch/notepad2.html) |
| notepadplusplus-pm | 1.4.12 | [https://bruderste.in/npp/pm/](https://bruderste.in/npp/pm/) |
| notepadplusplus | 7.6 | [https://notepad-plus-plus.org/](https://notepad-plus-plus.org/) |
| now-cli | 12.1.11 | [https://zeit.co/now](https://zeit.co/now) |
| nsis | 3.03 | [http://nsis.sourceforge.net/](http://nsis.sourceforge.net/) |
| nssm | 2.24 | [https://nssm.cc](https://nssm.cc) |
| nteract | 0.12.3 | [https://nteract.io/](https://nteract.io/) |
| nuget-package-explorer | 5.0.116 | [https://github.com/NuGetPackageExplorer/NuGetPackageExplorer](https://github.com/NuGetPackageExplorer/NuGetPackageExplorer) |
| nuget | 4.8.1 | [https://www.nuget.org/](https://www.nuget.org/) |
| nvm | 1.1.7 | [https://github.com/coreybutler/nvm-windows](https://github.com/coreybutler/nvm-windows) |
| nwjs-sdk | 0.35.1 | [https://nwjs.io/](https://nwjs.io/) |
| nwjs | 0.35.1 | [https://nwjs.io/](https://nwjs.io/) |
| obs-studio-small | 21.1.2 | [https://obsproject.com/](https://obsproject.com/) |
| obs-studio | 22.0.2 | [https://obsproject.com/](https://obsproject.com/) |
| ocenaudio | 3.5.4 | [https://www.ocenaudio.com/](https://www.ocenaudio.com/) |
| octave | 4.4.1 | [https://www.gnu.org/software/octave/](https://www.gnu.org/software/octave/) |
| oh-my-posh | 2.0.230 | [https://github.com/JanDeDobbeleer/oh-my-posh](https://github.com/JanDeDobbeleer/oh-my-posh) |
| omnisharp | 1.32.8 | [http://www.omnisharp.net](http://www.omnisharp.net) |
| onefetch | 1.0.0 | [https://github.com/o2sh/onefetch](https://github.com/o2sh/onefetch) |
| oneget | nightly | [https://oneget.org](https://oneget.org) |
| oni | 0.3.6 | [https://www.onivim.io/](https://www.onivim.io/) |
| openhab | 2.3.0 | [https://www.openhab.org/](https://www.openhab.org/) |
| openhardwaremonitor | 0.8.0 | [http://openhardwaremonitor.org/](http://openhardwaremonitor.org/) |
| openliberty | 18.0.0.3 | [https://openliberty.io/](https://openliberty.io/) |
| openresty | 1.13.6.2 | [https://github.com/openresty/openresty/blob/master/doc/README-win32.md#readme](https://github.com/openresty/openresty/blob/master/doc/README-win32.md#readme) |
| openshift-origin-client | 3.11.0 | [https://www.openshift.org](https://www.openshift.org) |
| openssh | 7.6p1 | [https://www.openssh.com/](https://www.openssh.com/) |
| openssl-slp | 1.1.0j | [https://slproweb.com/products/Win32OpenSSL.html](https://slproweb.com/products/Win32OpenSSL.html) |
| openssl | 1.1.1a | [https://curl.haxx.se/windows/](https://curl.haxx.se/windows/) |
| opentrack | 2.3.10 | [https://github.com/opentrack/opentrack](https://github.com/opentrack/opentrack) |
| openvpn | 2.4.6-I602 | [https://openvpn.net/](https://openvpn.net/) |
| opera | 57.0.3098.91 | [https://www.opera.com/](https://www.opera.com/) |
| optipng | 0.7.7 | [http://optipng.sourceforge.net/](http://optipng.sourceforge.net/) |
| orca | 3.1.4000.1830 | [https://msdn.microsoft.com/en-us/library/windows/desktop/aa370557(v=vs.85).aspx](https://msdn.microsoft.com/en-us/library/windows/desktop/aa370557(v=vs.85).aspx) |
| outlook-google-calendar-sync | 2.7.7-alpha | [https://phw198.github.io/OutlookGoogleCalendarSync/](https://phw198.github.io/OutlookGoogleCalendarSync/) |
| oxipng | 2.1.8 | [https://github.com/shssoichiro/oxipng](https://github.com/shssoichiro/oxipng) |
| p4merge | 152.131.2139 | [https://www.perforce.com/](https://www.perforce.com/) |
| packer | 1.3.3 | [https://www.packer.io](https://www.packer.io) |
| paint.net | 4.1.5 | [https://www.getpaint.net/](https://www.getpaint.net/) |
| palemoon-portable | 28.2.2 | [https://www.palemoon.org/](https://www.palemoon.org/) |
| palemoon | 28.2.2 | [https://www.palemoon.org/](https://www.palemoon.org/) |
| pandoc-crossref | 0.3.4.0 | [https://hackage.haskell.org/package/pandoc-crossref](https://hackage.haskell.org/package/pandoc-crossref) |
| pandoc | 2.5 | [https://pandoc.org/](https://pandoc.org/) |
| papdesigner | 2.2.0.8.04 | [http://friedrich-folkmann.de/papdesigner/Hauptseite.html](http://friedrich-folkmann.de/papdesigner/Hauptseite.html) |
| patch | 2.6.1 | [http://www.mingw.org/wiki/MSYS](http://www.mingw.org/wiki/MSYS) |
| patheditor | 1.0 | [https://patheditor2.codeplex.com/](https://patheditor2.codeplex.com/) |
| pathod | 4.0.4 | [https://mitmproxy.org/](https://mitmproxy.org/) |
| pcem | 14 | [https://pcem-emulator.co.uk/](https://pcem-emulator.co.uk/) |
| pci-z | 2.0-2017.07.01 | [https://www.pci-z.com/](https://www.pci-z.com/) |
| pciutils | 3.5.5 | [https://eternallybored.org/misc/pciutils/](https://eternallybored.org/misc/pciutils/) |
| pcregrep | 10.20 | [https://pcre.org/](https://pcre.org/) |
| pdf2djvu | 0.9.8 | [https://jwilk.net/software/pdf2djvu](https://jwilk.net/software/pdf2djvu) |
| pdfsam | 3.3.7 | [https://github.com/torakiki/pdfsam](https://github.com/torakiki/pdfsam) |
| pdftk | 2.02 | [https://www.pdflabs.com/tools/pdftk-server/](https://www.pdflabs.com/tools/pdftk-server/) |
| peco | 0.5.3 | [https://github.com/peco/peco/](https://github.com/peco/peco/) |
| peerblock | 1.1.691 | [https://forums.peerblock.com/](https://forums.peerblock.com/) |
| pentaho-data-integration | 8.2.0.0-342 | [https://pentaho.sourceforge.io/](https://pentaho.sourceforge.io/) |
| perl | 5.28.1.1 | [http://strawberryperl.com](http://strawberryperl.com) |
| persepolis | 3.1.0 | [https://persepolisdm.github.io/](https://persepolisdm.github.io/) |
| pester | 4.4.3 | [https://github.com/pester/Pester](https://github.com/pester/Pester) |
| phantomjs | 2.1.1 | [http://phantomjs.org/](http://phantomjs.org/) |
| php-nts-xdebug | 2.6.1-7.2 | [https://xdebug.org/](https://xdebug.org/) |
| php-nts | 7.2.13 | [http://windows.php.net](http://windows.php.net) |
| php-xdebug | 2.6.1-7.2 | [https://xdebug.org/](https://xdebug.org/) |
| php | 7.2.13 | [http://windows.php.net](http://windows.php.net) |
| picard | 2.0.4 | [https://picard.musicbrainz.org/](https://picard.musicbrainz.org/) |
| picotorrent | 0.15.0 | [https://picotorrent.org](https://picotorrent.org) |
| pixie | 4.1 | [http://www.nattyware.com/pixie.php](http://www.nattyware.com/pixie.php) |
| pkg-config | 0.26-1 | [https://www.freedesktop.org/wiki/Software/pkg-config/](https://www.freedesktop.org/wiki/Software/pkg-config/) |
| plantuml | 1.2018.13 | [http://plantuml.com/](http://plantuml.com/) |
| png2html | 1.1 | [https://www.engr.mun.ca/~holden/png2html.html](https://www.engr.mun.ca/~holden/png2html.html) |
| png2jpeg | 1.0.1.7 | [http://passgenwin.sourceforge.net/abpage/projects.xhtml#png2jpeg](http://passgenwin.sourceforge.net/abpage/projects.xhtml#png2jpeg) |
| pngcrush | 1.8.11 | [https://pmt.sourceforge.io/pngcrush/](https://pmt.sourceforge.io/pngcrush/) |
| pngquant | 2.12.1 | [https://pngquant.org/](https://pngquant.org/) |
| poppler | 0.68.0 | [http://blog.alivate.com.au/poppler-windows/](http://blog.alivate.com.au/poppler-windows/) |
| portainer | 1.19.2 | [https://portainer.io/](https://portainer.io/) |
| posh-docker | 0.7.0 | [https://github.com/samneirinck/posh-docker](https://github.com/samneirinck/posh-docker) |
| posh-git | 0.7.1 | [http://dahlbyk.github.io/posh-git/](http://dahlbyk.github.io/posh-git/) |
| postgresql | 11.1 | [https://www.postgresql.org/](https://www.postgresql.org/) |
| postman | 6.6.1 | [https://www.getpostman.com/](https://www.getpostman.com/) |
| potrace | 1.15 | [http://potrace.sourceforge.net/](http://potrace.sourceforge.net/) |
| powerping | 1.2.0 | [https://github.com/Killeroo/PowerPing](https://github.com/Killeroo/PowerPing) |
| powertab | 1.1.0 | [https://github.com/jasonmarcher/PowerTab](https://github.com/jasonmarcher/PowerTab) |
| ppsspp | 1.7.4 | [https://www.ppsspp.org](https://www.ppsspp.org) |
| premake4 | 4.4-b5 | [https://premake.github.io/download.html](https://premake.github.io/download.html) |
| premake5 | 5.0.0-alpha13 | [https://premake.github.io/](https://premake.github.io/) |
| process-explorer | 16.22 | [https://docs.microsoft.com/en-us/sysinternals/downloads/process-explorer](https://docs.microsoft.com/en-us/sysinternals/downloads/process-explorer) |
| process-explorer64 | 16.22 | [https://docs.microsoft.com/en-us/sysinternals/downloads/process-explorer](https://docs.microsoft.com/en-us/sysinternals/downloads/process-explorer) |
| processhacker | 2.39 | [http://processhacker.sourceforge.net/](http://processhacker.sourceforge.net/) |
| procexp | 16.22 | [https://docs.microsoft.com/en-us/sysinternals/downloads/process-explorer](https://docs.microsoft.com/en-us/sysinternals/downloads/process-explorer) |
| procexp64 | 16.22 | [https://docs.microsoft.com/en-us/sysinternals/downloads/process-explorer](https://docs.microsoft.com/en-us/sysinternals/downloads/process-explorer) |
| prometheus | 2.5.0 | [https://prometheus.io/](https://prometheus.io/) |
| protobuf | 3.6.1 | [https://github.com/google/protobuf](https://github.com/google/protobuf) |
| proxifier-portable | 3.42 | [https://www.proxifier.com](https://www.proxifier.com) |
| psake | 4.7.4 | [https://github.com/psake/psake](https://github.com/psake/psake) |
| psgithub | 2017.01.22 | []() |
| pshazz | 0.2018.09.25 | [https://github.com/lukesampson/pshazz](https://github.com/lukesampson/pshazz) |
| psiphon3 | 136 | [https://s3.amazonaws.com/psiphon/web/60l3-nnss-6gsn/index.html](https://s3.amazonaws.com/psiphon/web/60l3-nnss-6gsn/index.html) |
| PSPad | 5.0.0 | [http://www.pspad.com](http://www.pspad.com) |
| psutils | 0.2018.08.04 | [https://github.com/lukesampson/psutils](https://github.com/lukesampson/psutils) |
| pt | 2.2.0 | [https://github.com/monochromegane/the_platinum_searcher](https://github.com/monochromegane/the_platinum_searcher) |
| pup | 0.4.0 | [https://github.com/ericchiang/pup](https://github.com/ericchiang/pup) |
| puppet | 5.5.8 | [https://puppetlabs.com](https://puppetlabs.com) |
| purescript | 0.12.1 | [http://purescript.org/](http://purescript.org/) |
| putty | 0.70 | [https://www.chiark.greenend.org.uk/~sgtatham/putty/](https://www.chiark.greenend.org.uk/~sgtatham/putty/) |
| pwsafe | 3.47.2 | [https://pwsafe.org/](https://pwsafe.org/) |
| pwsh | 6.1.1 | [https://github.com/PowerShell/PowerShell](https://github.com/PowerShell/PowerShell) |
| px | 2018-05-18 | [https://github.com/genotrance/px](https://github.com/genotrance/px) |
| pycharm | 2018.3.1 | [https://www.jetbrains.com/pycharm/](https://www.jetbrains.com/pycharm/) |
| pychess | 0.99.3 | [http://pychess.org/](http://pychess.org/) |
| pypy2 | 6.0.0 | [https://pypy.org](https://pypy.org) |
| python-exp | 3.5.2 | [https://www.python.org/](https://www.python.org/) |
| python | 3.7.1 | [https://www.python.org/](https://www.python.org/) |
| python27 | 2.7.15 | [https://www.python.org/](https://www.python.org/) |
| python35 | 3.5.4 | [https://www.python.org/](https://www.python.org/) |
| qaac | 2.68 | [https://sites.google.com/site/qaacpage/](https://sites.google.com/site/qaacpage/) |
| qbittorrent | 4.1.4 | [https://www.qbittorrent.org/](https://www.qbittorrent.org/) |
| qemu | 3.1.0 | [https://qemu.weilnetz.de/](https://qemu.weilnetz.de/) |
| qnapi | 0.2.3 | [https://qnapi.github.io/](https://qnapi.github.io/) |
| qpdf | 8.2.1 | [http://qpdf.sourceforge.net/](http://qpdf.sourceforge.net/) |
| qrencode | 3.4.4 | [https://code.google.com/archive/p/qrencode-win32/](https://code.google.com/archive/p/qrencode-win32/) |
| quicklook | 3.6.4 | [https://pooi.moe/QuickLook/](https://pooi.moe/QuickLook/) |
| quiterss | 0.18.12 | [https://quiterss.org/en](https://quiterss.org/en) |
| qutebrowser | 1.5.2 | [https://www.qutebrowser.org/](https://www.qutebrowser.org/) |
| r | 3.5.1 | [https://www.r-project.org](https://www.r-project.org) |
| rabbitmq | 3.7.9 | [https://www.rabbitmq.com/](https://www.rabbitmq.com/) |
| rabbitmqadmin | 3.7.9 | [https://www.rabbitmq.com/management-cli.html](https://www.rabbitmq.com/management-cli.html) |
| racket | 7.1 | [https://racket-lang.org](https://racket-lang.org) |
| radare2 | 3.1.3 | [https://www.radare.org/r/](https://www.radare.org/r/) |
| ragel | 6.9 | [https://github.com/eloraiby/ragel-windows](https://github.com/eloraiby/ragel-windows) |
| rainmeter | 4.2.0.3111 | [https://rainmeter.net/](https://rainmeter.net/) |
| rambox-pro | 1.0.8 | [https://rambox.pro/](https://rambox.pro/) |
| rambox | 0.6.3 | [http://rambox.pro/](http://rambox.pro/) |
| rancher-compose | 0.12.5 | [https://rancher.com/](https://rancher.com/) |
| rapidee | 937 | [https://www.rapidee.com/en/about](https://www.rapidee.com/en/about) |
| rcedit | 1.1.1 | [https://github.com/electron/rcedit](https://github.com/electron/rcedit) |
| rclone | 1.45 | [https://rclone.org](https://rclone.org) |
| reaper | 5.963 | [https://www.reaper.fm](https://www.reaper.fm) |
| recuva | 1.53.1087 | [https://www.ccleaner.com/recuva](https://www.ccleaner.com/recuva) |
| red | 0.6.4 | [http://www.red-lang.org](http://www.red-lang.org) |
| redis | 3.2.100 | [https://redis.io](https://redis.io) |
| renderdoc | 1.2 | [https://renderdoc.org](https://renderdoc.org) |
| reshade | 4.0.2 | [https://reshade.me/](https://reshade.me/) |
| resharper-clt | 2018.2.3 | [https://www.jetbrains.com/resharper/download/index.html#section=resharper-clt](https://www.jetbrains.com/resharper/download/index.html#section=resharper-clt) |
| resource-hacker | 5.1.6 | [http://www.angusj.com/resourcehacker/](http://www.angusj.com/resourcehacker/) |
| restic | 0.9.3 | [https://restic.github.io/](https://restic.github.io/) |
| rethinkdb | 2.3.6 | [https://www.rethinkdb.com/](https://www.rethinkdb.com/) |
| retroarch | 1.7.5 | [http://www.retroarch.com/](http://www.retroarch.com/) |
| ripgrep | 0.10.0 | [https://github.com/BurntSushi/ripgrep](https://github.com/BurntSushi/ripgrep) |
| ripme | 1.7.72 | [https://github.com/RipMeApp/ripme](https://github.com/RipMeApp/ripme) |
| rktools2k3 | 1.0 | [https://github.com/kodybrown/rktools2k3](https://github.com/kodybrown/rktools2k3) |
| robo3t | 1.2.1 | [https://robomongo.org](https://robomongo.org) |
| rstudio | 1.1.463 | [https://www.rstudio.com/](https://www.rstudio.com/) |
| rtmpdump | 2.3 | [https://rtmpdump.mplayerhq.hu/](https://rtmpdump.mplayerhq.hu/) |
| ruby | 2.4.5-1 | [https://rubyinstaller.org](https://rubyinstaller.org) |
| rufus | 3.4 | [https://rufus.ie/](https://rufus.ie/) |
| runat | 0.2018.08.04 | [https://github.com/lukesampson/psutils](https://github.com/lukesampson/psutils) |
| rust-msvc-nightly | nightly | [https://www.rust-lang.org](https://www.rust-lang.org) |
| rust-msvc | 1.30.1 | [https://www.rust-lang.org](https://www.rust-lang.org) |
| rust-nightly | nightly | [https://www.rust-lang.org](https://www.rust-lang.org) |
| rust | 1.30.1 | [https://www.rust-lang.org](https://www.rust-lang.org) |
| rustup | 1.16.0 | [https://github.com/rust-lang-nursery/rustup.rs](https://github.com/rust-lang-nursery/rustup.rs) |
| rxrepl | 1.5 | [https://sites.google.com/site/regexreplace/](https://sites.google.com/site/regexreplace/) |
| s | 0.5.13 | [https://github.com/zquestz/s](https://github.com/zquestz/s) |
| s3deploy | 2.2.0 | []() |
| sabnzbd | 2.3.5 | [https://sabnzbd.org/](https://sabnzbd.org/) |
| sacad | 2.1.7 | [https://github.com/desbma/sacad](https://github.com/desbma/sacad) |
| sandman | 1.9.2 | [https://alexanderepstein.github.io/Sandman/](https://alexanderepstein.github.io/Sandman/) |
| sass | 1.15.2 | [https://github.com/sass/dart-sass](https://github.com/sass/dart-sass) |
| say | 0.2018.08.04 | [https://github.com/lukesampson/psutils](https://github.com/lukesampson/psutils) |
| sbcl | 1.4.14 | [http://www.sbcl.org/](http://www.sbcl.org/) |
| sbt | 1.2.7 | [https://www.scala-sbt.org/](https://www.scala-sbt.org/) |
| scala | 2.12.8 | [https://www.scala-lang.org/](https://www.scala-lang.org/) |
| scallion | 2.1 | [https://github.com/lachesis/scallion](https://github.com/lachesis/scallion) |
| scholdoc | 0.1.3 | [http://scholdoc.scholarlymarkdown.com/](http://scholdoc.scholarlymarkdown.com/) |
| scons | 3.0.1 | [https://scons.org/](https://scons.org/) |
| scrcpy | 1.5 | [https://github.com/Genymobile/scrcpy](https://github.com/Genymobile/scrcpy) |
| screentogif | 2.14.1 | [http://www.screentogif.com/](http://www.screentogif.com/) |
| scriptcs | 0.17.1 | [http://scriptcs.net/](http://scriptcs.net/) |
| sdl2 | 2.0.7 | [https://www.libsdl.org](https://www.libsdl.org) |
| sed | 4.2.1 | [http://gnuwin32.sourceforge.net/packages/sed.htm](http://gnuwin32.sourceforge.net/packages/sed.htm) |
| selenium | 3.141.59 | [http://www.seleniumhq.org/](http://www.seleniumhq.org/) |
| sendemail | 156 | [http://caspian.dotconf.net/menu/Software/SendEmail/](http://caspian.dotconf.net/menu/Software/SendEmail/) |
| seqcli | 5.0.165 | [https://github.com/datalust/seqcli](https://github.com/datalust/seqcli) |
| serve | 0.2.1 | [https://github.com/philippgille/serve](https://github.com/philippgille/serve) |
| servicebusexplorer | 4.0.110 | [https://github.com/paolosalvatori/ServiceBusExplorer](https://github.com/paolosalvatori/ServiceBusExplorer) |
| sfk | 1.9.3.4 | [http://stahlworks.com/dev/swiss-file-knife.html](http://stahlworks.com/dev/swiss-file-knife.html) |
| shadowsocks | 4.1.2 | [https://github.com/shadowsocks/shadowsocks-windows](https://github.com/shadowsocks/shadowsocks-windows) |
| shadowsocksr-csharp | 4.9.0 | [https://github.com/shadowsocksrr/shadowsocksr-csharp](https://github.com/shadowsocksrr/shadowsocksr-csharp) |
| sharex | 12.3.1 | [https://getsharex.com/](https://getsharex.com/) |
| sharpkeys | 3.8 | [https://github.com/randyrants/sharpkeys](https://github.com/randyrants/sharpkeys) |
| shasum | 0.2018.08.04 | [https://github.com/lukesampson/psutils](https://github.com/lukesampson/psutils) |
| shellcheck | 0.6.0 | [https://shellcheck.net/](https://shellcheck.net/) |
| shim | 0.2013.11.19 | [https://github.com/lukesampson/psutils](https://github.com/lukesampson/psutils) |
| shinjiru | 3.3.2 | [https://shinjiru.me/](https://shinjiru.me/) |
| signal | 1.19.0 | [https://signal.org/](https://signal.org/) |
| simplewall | 2.3.10 | [https://www.henrypp.org/product/simplewall](https://www.henrypp.org/product/simplewall) |
| skaffold | 0.19.0 | [https://github.com/GoogleCloudPlatform/skaffold](https://github.com/GoogleCloudPlatform/skaffold) |
| slack | 3.3.3 | [https://slack.com/downloads/windows](https://slack.com/downloads/windows) |
| sliksvn | 1.9.7 | [https://sliksvn.com/](https://sliksvn.com/) |
| smartmontools | 6.6-1 | [https://www.smartmontools.org/](https://www.smartmontools.org/) |
| smartty | 3.1 | [http://smartty.sysprogs.com/](http://smartty.sysprogs.com/) |
| snaketail | 1.9.4 | [http://snakenest.com/snaketail/](http://snakenest.com/snaketail/) |
| snipaste | 1.16.2 | [https://www.snipaste.com/](https://www.snipaste.com/) |
| soapui | 5.4.0 | [https://www.soapui.org/](https://www.soapui.org/) |
| solidity | 0.5.1 | [https://solidity.readthedocs.io](https://solidity.readthedocs.io) |
| sonarqube | 7.4 | [https://www.sonarqube.org](https://www.sonarqube.org) |
| soulseekqt | 2017-2-20 | [http://www.slsknet.org/news/node/1](http://www.slsknet.org/news/node/1) |
| sourcetree | 3.0.12 | [https://www.sourcetreeapp.com/](https://www.sourcetreeapp.com/) |
| SpaceSniffer | 1.3.0.2 | [http://www.uderzo.it/main_products/space_sniffer/index.html](http://www.uderzo.it/main_products/space_sniffer/index.html) |
| spark | 2.4.0 | [https://spark.apache.org/](https://spark.apache.org/) |
| speccy | 1.32.740 | [https://www.piriform.com/speccy](https://www.piriform.com/speccy) |
| speedcrunch | 0.12 | [http://speedcrunch.org/](http://speedcrunch.org/) |
| speedfan | 4.52 | [http://www.almico.com/speedfan.php](http://www.almico.com/speedfan.php) |
| speedyfox | 2.0.25 | [https://www.crystalidea.com/speedyfox](https://www.crystalidea.com/speedyfox) |
| springboot | 2.1.1 | [https://projects.spring.io/spring-boot/](https://projects.spring.io/spring-boot/) |
| spytify | 1.1.3.1 | [https://github.com/jwallet/spy-spotify](https://github.com/jwallet/spy-spotify) |
| sqlite | 3.26.0 | [https://www.sqlite.org/](https://www.sqlite.org/) |
| sqlitebrowser | 3.10.1 | [http://sqlitebrowser.org/](http://sqlitebrowser.org/) |
| sqlitestudio | 3.2.1 | [https://sqlitestudio.pl/index.rvt](https://sqlitestudio.pl/index.rvt) |
| sqlopsstudio | 0.33.7 | [https://docs.microsoft.com/en-us/sql/sql-operations-studio](https://docs.microsoft.com/en-us/sql/sql-operations-studio) |
| squashfs-tools | 43 | [https://github.com/pmq20/squashfuse](https://github.com/pmq20/squashfuse) |
| srvman | 1.0 | [http://tools.sysprogs.org/srvman/](http://tools.sysprogs.org/srvman/) |
| ssd-z | 16.09.09 | [http://aezay.dk/aezay/ssdz/](http://aezay.dk/aezay/ssdz/) |
| ssh-copy-id | 2015-03-22 | [https://github.com/VijayS1/Scripts/blob/master/ssh-copy-id/README.md](https://github.com/VijayS1/Scripts/blob/master/ssh-copy-id/README.md) |
| sslscan | 1.11.11 | [https://github.com/rbsec/sslscan](https://github.com/rbsec/sslscan) |
| stack | 1.9.3 | [https://www.haskellstack.org](https://www.haskellstack.org) |
| station | 1.31.3 | [https://getstation.com/](https://getstation.com/) |
| steam-library-manager | 1.5.0.12 | [https://github.com/RevoLand/Steam-Library-Manager](https://github.com/RevoLand/Steam-Library-Manager) |
| steam | nightly | [https://store.steampowered.com/](https://store.steampowered.com/) |
| steamcmd | 1532461524 | [https://developer.valvesoftware.com/wiki/SteamCMD](https://developer.valvesoftware.com/wiki/SteamCMD) |
| stone-soup-tiles | 0.22.1 | [https://crawl.develz.org/](https://crawl.develz.org/) |
| stone-soup | 0.22.1 | [https://crawl.develz.org/](https://crawl.develz.org/) |
| storageexplorer | 1.5.0 | [https://azure.microsoft.com/en-us/features/storage-explorer/](https://azure.microsoft.com/en-us/features/storage-explorer/) |
| streamlink | 0.14.2 | [https://streamlink.github.io/](https://streamlink.github.io/) |
| strokesplus-portable | 2.8.6.4 | [https://www.strokesplus.com](https://www.strokesplus.com) |
| sts | 3.9.6 | [https://spring.io/tools/sts](https://spring.io/tools/sts) |
| stunnel | 5.49 | [https://www.stunnel.org](https://www.stunnel.org) |
| sublime-merge | 1097 | [https://www.sublimemerge.com/](https://www.sublimemerge.com/) |
| sublime-text | 3176 | [https://www.sublimetext.com/3](https://www.sublimetext.com/3) |
| subtitleedit | 3.5.7 | [http://www.nikse.dk/subtitleedit/](http://www.nikse.dk/subtitleedit/) |
| sudo | 0.2018.08.04 | [https://github.com/lukesampson/psutils](https://github.com/lukesampson/psutils) |
| sumatrapdf | 3.1.2 | [https://www.sumatrapdfreader.org](https://www.sumatrapdfreader.org) |
| sunsetscreen | 1.30 | [http://www.skytopia.com/software/sunsetscreen/](http://www.skytopia.com/software/sunsetscreen/) |
| svcat | 0.1.38 | [https://svc-cat.io/](https://svc-cat.io/) |
| svtplay-dl | 2.1 | [https://svtplay-dl.se/](https://svtplay-dl.se/) |
| sweethome3d | 6.0 | [http://www.sweethome3d.com/](http://www.sweethome3d.com/) |
| swig | 3.0.12 | [http://www.swig.org](http://www.swig.org) |
| syncany-cli | 0.4.9 | [https://www.syncany.org/](https://www.syncany.org/) |
| syncbackpro | 8.5.97.0 | [https://www.2brightsparks.com/syncback/sbpro.html](https://www.2brightsparks.com/syncback/sbpro.html) |
| syncthing | 0.14.54 | [https://syncthing.net/](https://syncthing.net/) |
| synctrayzor | 1.1.22 | [https://github.com/canton7/SyncTrayzor](https://github.com/canton7/SyncTrayzor) |
| sysinternals | July.5.2018 | [https://docs.microsoft.com/en-us/sysinternals/](https://docs.microsoft.com/en-us/sysinternals/) |
| taiga | 1.3.1 | [http://taiga.moe/](http://taiga.moe/) |
| tar | 1.23 | [http://www.mingw.org/wiki/msys](http://www.mingw.org/wiki/msys) |
| task | 2.2.1 | [https://taskfile.org](https://taskfile.org) |
| tcc | 0.9.26 | [https://bellard.org/tcc/](https://bellard.org/tcc/) |
| tcpipmanager | 4.1.1 | [http://tcpipmanager.sourceforge.net](http://tcpipmanager.sourceforge.net) |
| teamspeak3 | 3.2.3 | [https://www.teamspeak.com/en/](https://www.teamspeak.com/en/) |
| teamviewer | 14.0.13880 | [https://www.teamviewer.com](https://www.teamviewer.com) |
| telegram | 1.5.1 | [https://telegram.org/](https://telegram.org/) |
| telnet | msys-inetutils-1.7-1 | [http://www.mingw.org/wiki/msys](http://www.mingw.org/wiki/msys) |
| terminals | 4.0.1 | [https://github.com/Terminals-Origin/Terminals](https://github.com/Terminals-Origin/Terminals) |
| terminus | 1.0.65 | [https://eugeny.github.io/terminus/](https://eugeny.github.io/terminus/) |
| terraform | 0.11.10 | [https://www.terraform.io](https://www.terraform.io) |
| terragrunt | 0.17.3 | [https://github.com/gruntwork-io/terragrunt](https://github.com/gruntwork-io/terragrunt) |
| tesseract | 4.0.0.20181030 | [https://github.com/UB-Mannheim/tesseract/wiki](https://github.com/UB-Mannheim/tesseract/wiki) |
| texmaker | 5.0.3 | [http://www.xm1math.net/texmaker/](http://www.xm1math.net/texmaker/) |
| texstudio | 2.12.14 | [https://www.texstudio.org](https://www.texstudio.org) |
| textadept | 10.2 | [https://foicica.com/textadept/](https://foicica.com/textadept/) |
| texteditoranywhere | 2.01 | [https://www.listary.com/text-editor-anywhere](https://www.listary.com/text-editor-anywhere) |
| thrift | 0.11.0 | [https://thrift.apache.org/](https://thrift.apache.org/) |
| thunderbird | 60.3.3 | [https://www.mozilla.org/en-US/thunderbird/](https://www.mozilla.org/en-US/thunderbird/) |
| tidy | 5.6.0 | [http://www.html-tidy.org/](http://www.html-tidy.org/) |
| time | 0.2018.08.04 | [https://github.com/lukesampson/psutils](https://github.com/lukesampson/psutils) |
| todolist | 7.1.5.0 | [https://abstractspoon.weebly.com/](https://abstractspoon.weebly.com/) |
| tomcat | 9.0.12 | [https://tomcat.apache.org/](https://tomcat.apache.org/) |
| tor-browser | 8.0.4 | [https://www.torproject.org/](https://www.torproject.org/) |
| tor-expert | 0.3.4.9 | [https://www.torproject.org](https://www.torproject.org) |
| tortoisemerge | 1.6.7 | [https://tortoisesvn.net/TortoiseMerge.html](https://tortoisesvn.net/TortoiseMerge.html) |
| tortoisesvn | 1.11.0.28416 | [https://tortoisesvn.net](https://tortoisesvn.net) |
| totalcommander | 9.21a | [https://www.ghisler.com](https://www.ghisler.com) |
| touch | 0.2018.08.04 | [https://github.com/lukesampson/psutils](https://github.com/lukesampson/psutils) |
| traefik | 1.7.5 | [https://traefik.io/](https://traefik.io/) |
| transmission-cli | 2.94 | [https://transmissionbt.com/](https://transmissionbt.com/) |
| transmission | 2.94 | [https://transmissionbt.com/](https://transmissionbt.com/) |
| tremulous | 1.3.0-alpha.0.13 | [http://tremulous.net/](http://tremulous.net/) |
| trid | 2.24-18.12.11 | [http://mark0.net/soft-trid-e.html](http://mark0.net/soft-trid-e.html) |
| tunnel | 0.2.12 | [https://github.com/labstack/tunnel-client](https://github.com/labstack/tunnel-client) |
| tup | 0.7.8 | [http://gittup.org](http://gittup.org) |
| UIforETW | 1.50 | [https://github.com/google/UIforETW](https://github.com/google/UIforETW) |
| unar | 1.8.1 | [https://theunarchiver.com/command-line](https://theunarchiver.com/command-line) |
| unbound | 1.8.3 | [https://unbound.net/](https://unbound.net/) |
| uncap | 0.2.2 | [https://github.com/susam/uncap](https://github.com/susam/uncap) |
| uncrustify | 0.68.1 | [http://uncrustify.sourceforge.net/](http://uncrustify.sourceforge.net/) |
| unetbootin | 661 | [https://unetbootin.github.io](https://unetbootin.github.io) |
| ungoogled-chromium | 67.0.3396.87-3 | [https://github.com/Eloston/ungoogled-chromium](https://github.com/Eloston/ungoogled-chromium) |
| universalpausebutton | 1.0.3 | [https://github.com/ryanries/UniversalPauseButton](https://github.com/ryanries/UniversalPauseButton) |
| unlocker | 1.9.0 | [http://www.emptyloop.com/unlocker](http://www.emptyloop.com/unlocker) |
| unrar | 5.61 | [https://www.rarlab.com/](https://www.rarlab.com/) |
| unzip | 6.00 | [http://www.info-zip.org/](http://www.info-zip.org/) |
| up | 0.8.1 | [https://github.com/apex/up](https://github.com/apex/up) |
| upx | 3.95 | [https://upx.github.io/](https://upx.github.io/) |
| usql | 0.7.0 | [https://github.com/xo/usql](https://github.com/xo/usql) |
| util-linux-ng | 2.14.1 | [http://gnuwin32.sourceforge.net/packages/util-linux-ng.htm](http://gnuwin32.sourceforge.net/packages/util-linux-ng.htm) |
| vagrant | 2.2.2 | [https://www.vagrantup.com/](https://www.vagrantup.com/) |
| vault | 1.0.0 | [https://www.vaultproject.io](https://www.vaultproject.io) |
| vbindiff | 3.0-beta5 | [https://www.cjmweb.net/vbindiff/](https://www.cjmweb.net/vbindiff/) |
| vcredist | 14.10.25008 | [https://www.visualstudio.com/de/downloads/](https://www.visualstudio.com/de/downloads/) |
| vcredist2008 | 9.0.30729 | [https://support.microsoft.com/en-us/help/2977003/the-latest-supported-visual-c-downloads](https://support.microsoft.com/en-us/help/2977003/the-latest-supported-visual-c-downloads) |
| vcredist2010 | 10.0.40219 | [https://support.microsoft.com/en-us/help/2977003/the-latest-supported-visual-c-downloads](https://support.microsoft.com/en-us/help/2977003/the-latest-supported-visual-c-downloads) |
| vcredist2012 | 11.0.61030 | [https://support.microsoft.com/en-us/help/2977003/the-latest-supported-visual-c-downloads](https://support.microsoft.com/en-us/help/2977003/the-latest-supported-visual-c-downloads) |
| vcredist2013 | 12.0.40660 | [https://support.microsoft.com/en-us/help/2977003/the-latest-supported-visual-c-downloads](https://support.microsoft.com/en-us/help/2977003/the-latest-supported-visual-c-downloads) |
| vcredist2015 | 14.0.24215 | [https://support.microsoft.com/en-us/help/2977003/the-latest-supported-visual-c-downloads](https://support.microsoft.com/en-us/help/2977003/the-latest-supported-visual-c-downloads) |
| vcredist2017 | 14.10.25008 | [https://www.visualstudio.com/de/downloads/](https://www.visualstudio.com/de/downloads/) |
| vcxsrv | 1.20.1.4 | [https://vcxsrv.sourceforge.io/](https://vcxsrv.sourceforge.io/) |
| vifm | 0.10 | [https://vifm.info/](https://vifm.info/) |
| vim | 8.1.0577 | [http://www.vim.org](http://www.vim.org) |
| vimtutor | 0.2018.08.04 | [https://github.com/lukesampson/psutils](https://github.com/lukesampson/psutils) |
| visual-arm-emulator | 1.27 | [https://salmanarif.bitbucket.io/visual/index.html](https://salmanarif.bitbucket.io/visual/index.html) |
| visualc | 16.00.30319.01 | [https://www.visualstudio.com](https://www.visualstudio.com) |
| vivaldi | 2.1.1337.51 | [https://vivaldi.com/](https://vivaldi.com/) |
| vlc | 3.0.4 | [https://www.videolan.org/](https://www.videolan.org/) |
| vncviewer | 6.18.907 | [https://www.realvnc.com/download/viewer](https://www.realvnc.com/download/viewer) |
| vnote | 2.1 | [https://tamlok.github.io/vnote/](https://tamlok.github.io/vnote/) |
| vott | 1.7.1 | [https://github.com/Microsoft/VoTT](https://github.com/Microsoft/VoTT) |
| vscode-insiders-portable | nightly | [https://code.visualstudio.com/](https://code.visualstudio.com/) |
| vscode-insiders | nightly | [https://code.visualstudio.com/](https://code.visualstudio.com/) |
| vscode-portable | 1.29.1 | [https://code.visualstudio.com/](https://code.visualstudio.com/) |
| vscode | 1.29.1 | [https://code.visualstudio.com/](https://code.visualstudio.com/) |
| vswhere | 2.5.2 | [https://github.com/Microsoft/vswhere](https://github.com/Microsoft/vswhere) |
| warp | 0.3.0 | [https://github.com/dgiagio/warp](https://github.com/dgiagio/warp) |
| watchexec | 1.9.2 | [https://github.com/mattgreen/watchexec](https://github.com/mattgreen/watchexec) |
| watchman-nightly | nightly | [https://facebook.github.io/watchman/](https://facebook.github.io/watchman/) |
| wavebox | 4.5.5 | [https://wavebox.io/](https://wavebox.io/) |
| webpicmd | 4.5 | [https://docs.microsoft.com/en-us/iis/install/web-platform-installer/web-platform-installer-v4-command-line-webpicmdexe-rtw-release](https://docs.microsoft.com/en-us/iis/install/web-platform-installer/web-platform-installer-v4-command-line-webpicmdexe-rtw-release) |
| webstorm | 2018.3.1 | [https://www.jetbrains.com/webstorm/](https://www.jetbrains.com/webstorm/) |
| webtorrent | 0.20.0 | [https://webtorrent.io/desktop/](https://webtorrent.io/desktop/) |
| wget | 1.20 | [https://eternallybored.org/misc/wget/](https://eternallybored.org/misc/wget/) |
| whatsapp | 0.3.1649 | [https://www.whatsapp.com](https://www.whatsapp.com) |
| which | 2.20 | [http://gnuwin32.sourceforge.net/packages/which.htm](http://gnuwin32.sourceforge.net/packages/which.htm) |
| wifi-manager | 0.2 | [https://github.com/shanselman/Windows-Wifi-Manager](https://github.com/shanselman/Windows-Wifi-Manager) |
| win-acme | 1.9.12.2 | [https://github.com/PKISharp/win-acme](https://github.com/PKISharp/win-acme) |
| win-portacle | 1.2c | [https://portacle.github.io/](https://portacle.github.io/) |
| win32-disk-imager | 1.0.0 | [https://sourceforge.net/projects/win32diskimager/](https://sourceforge.net/projects/win32diskimager/) |
| win32-openssh | 7.7.2.0p1-Beta | [https://github.com/PowerShell/Win32-OpenSSH](https://github.com/PowerShell/Win32-OpenSSH) |
| winbox | 3.18 | [https://mikrotik.com/](https://mikrotik.com/) |
| wincdemu | 4.0 | [http://wincdemu.sysprogs.org/](http://wincdemu.sysprogs.org/) |
| wincompose | 0.8.2 | [http://wincompose.info/](http://wincompose.info/) |
| windirstat | 1.1.2 | [https://windirstat.net/](https://windirstat.net/) |
| windows-application-driver | 1.1 | [https://github.com/Microsoft/WinAppDriver](https://github.com/Microsoft/WinAppDriver) |
| winfile-original | 10.0 | [https://github.com/Microsoft/winfile](https://github.com/Microsoft/winfile) |
| winfile | 10.0.1806.1 | [https://github.com/Microsoft/winfile](https://github.com/Microsoft/winfile) |
| winmerge | 2.16.0 | [http://winmerge.org](http://winmerge.org) |
| winmerge2011 | 0.2011.008.313 | [https://bitbucket.org/jtuc/winmerge2011](https://bitbucket.org/jtuc/winmerge2011) |
| winpython | 3.6.7.0 | [https://winpython.github.io/](https://winpython.github.io/) |
| winrar | 5.61 | [https://rarlab.com/](https://rarlab.com/) |
| winscp | 5.13.6 | [https://winscp.net](https://winscp.net) |
| winyl | 3.3.1 | [http://vinylsoft.com/](http://vinylsoft.com/) |
| wireshark | 2.6.5 | [https://www.wireshark.org/](https://www.wireshark.org/) |
| wixtoolset | 3.11.1 | [http://wixtoolset.org/](http://wixtoolset.org/) |
| wiztree | 3.26 | [https://antibody-software.com/web/software/software/wiztree-finds-the-files-and-folders-using-the-most-disk-space-on-your-hard-drive](https://antibody-software.com/web/software/software/wiztree-finds-the-files-and-folders-using-the-most-disk-space-on-your-hard-drive) |
| wkhtmltopdf | 0.12.5-1 | [https://wkhtmltopdf.org/](https://wkhtmltopdf.org/) |
| wox | 1.3.524 | [http://www.wox.one/](http://www.wox.one/) |
| write | 1.0b8.4 | [https://wri.tt/](https://wri.tt/) |
| wsltty | 1.9.5 | [https://github.com/mintty/wsltty](https://github.com/mintty/wsltty) |
| wurl | 1.0.1 | [https://github.com/xakep666/wurl](https://github.com/xakep666/wurl) |
| wuzz | 0.4.0 | [https://github.com/asciimoo/wuzz](https://github.com/asciimoo/wuzz) |
| wxhexeditor | 0.24 | [http://www.wxhexeditor.org/](http://www.wxhexeditor.org/) |
| wyam | 2.1.0 | [https://wyam.io](https://wyam.io) |
| x264-10bit | 2851 | [https://www.videolan.org/developers/x264.html](https://www.videolan.org/developers/x264.html) |
| x264 | 2935 | [https://www.videolan.org/developers/x264.html](https://www.videolan.org/developers/x264.html) |
| x64dbg | 2018-11-27_12-40 | [https://x64dbg.com/](https://x64dbg.com/) |
| xdelta | 3.1.0 | [http://xdelta.org/](http://xdelta.org/) |
| xdman | 7.2.8 | [http://xdman.sourceforge.net/](http://xdman.sourceforge.net/) |
| xmake | 2.2.3 | [https://xmake.io](https://xmake.io) |
| xmedia-recode | 3.4.4.8 | [https://www.xmedia-recode.de/en/](https://www.xmedia-recode.de/en/) |
| xmind8 | 3.7.8 | [https://www.xmind.net/](https://www.xmind.net/) |
| xming | 6.9.0.31 | [http://www.straightrunning.com/XmingNotes/](http://www.straightrunning.com/XmingNotes/) |
| xmllint | 2.9.3 | [http://xmlsoft.org/](http://xmlsoft.org/) |
| xmlstarlet | 1.6.1 | [http://xmlstar.sourceforge.net/](http://xmlstar.sourceforge.net/) |
| xmousebuttoncontrol | 2.17 | [https://www.highrez.co.uk/downloads/xmousebuttoncontrol.htm](https://www.highrez.co.uk/downloads/xmousebuttoncontrol.htm) |
| xsv | 0.13.0 | [https://github.com/BurntSushi/xsv](https://github.com/BurntSushi/xsv) |
| xx-net | 3.12.11 | [https://github.com/XX-net/XX-Net](https://github.com/XX-net/XX-Net) |
| xyplorer | 17.40.0100 | [https://www.xyplorer.com/free.php](https://www.xyplorer.com/free.php) |
| xz | 5.2.4 | [https://tukaani.org/xz/](https://tukaani.org/xz/) |
| yara | 3.8.1 | [https://virustotal.github.io/yara/](https://virustotal.github.io/yara/) |
| yarn | 1.12.3 | [https://yarnpkg.com/](https://yarnpkg.com/) |
| yasm | 1.3.0 | [http://yasm.tortall.net/](http://yasm.tortall.net/) |
| yatqa | 3.9.5 | [http://yat.qa/](http://yat.qa/) |
| youtube-dl-gui | 0.4 | [https://github.com/MrS0m30n3/youtube-dl-gui](https://github.com/MrS0m30n3/youtube-dl-gui) |
| youtube-dl | 2018.12.09 | [https://rg3.github.io/youtube-dl/](https://rg3.github.io/youtube-dl/) |
| yubico-piv-tool | 1.6.2 | [https://developers.yubico.com/yubico-piv-tool/](https://developers.yubico.com/yubico-piv-tool/) |
| yubikey-manager-qt | 0.5.2 | [https://developers.yubico.com/yubikey-manager-qt/](https://developers.yubico.com/yubikey-manager-qt/) |
| yubikey-personalization-gui | 3.1.25 | [https://developers.yubico.com/yubikey-personalization-gui/](https://developers.yubico.com/yubikey-personalization-gui/) |
| yubikey-personalization | 1.19.0 | [https://developers.yubico.com/yubikey-personalization/](https://developers.yubico.com/yubikey-personalization/) |
| yubikey-piv-manager | 1.4.2 | [https://developers.yubico.com/yubikey-piv-manager/](https://developers.yubico.com/yubikey-piv-manager/) |
| zeal | 0.6.1 | [https://zealdocs.org/](https://zealdocs.org/) |
| zeppelin | 0.8.0 | [https://zeppelin.apache.org/](https://zeppelin.apache.org/) |
| zeronet | 0.6.4 | [https://zeronet.io/](https://zeronet.io/) |
| ziglang | 0.3.0 | [https://ziglang.org/](https://ziglang.org/) |
| zip | 3.0 | [http://www.info-zip.org/](http://www.info-zip.org/) |
| zlocation | 1.1.0 | [https://github.com/vors/ZLocation](https://github.com/vors/ZLocation) |
| zola | 0.5.0 | [https://www.getzola.org/](https://www.getzola.org/) |
| zookeeper | 3.4.13 | [https://zookeeper.apache.org/](https://zookeeper.apache.org/) |
| zstd | 1.3.7 | [http://www.zstd.net/](http://www.zstd.net/) |

This file was automatically generated.
