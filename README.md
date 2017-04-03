# api documentation for  [irc (v0.5.2)](https://github.com/martynsmith/node-irc#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-irc.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-irc) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-irc.svg)](https://travis-ci.org/npmdoc/node-npmdoc-irc)
#### An IRC client library for node

[![NPM](https://nodei.co/npm/irc.png?downloads=true)](https://www.npmjs.com/package/irc)

[![apidoc](https://npmdoc.github.io/node-npmdoc-irc/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-irc_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-irc/build..beta..travis-ci.org/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-irc/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-irc/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Martyn Smith",
        "email": "martyn@dollyfish.net.nz"
    },
    "bugs": {
        "url": "http://github.com/martynsmith/node-irc/issues"
    },
    "contributors": [
        {
            "name": "Fionn Kelleher",
            "email": "me@fionn.co"
        },
        {
            "name": "xAndy",
            "email": "xandy@hackerspace-bamberg.de"
        },
        {
            "name": "Mischa Spiegelmock",
            "email": "revmischa@cpan.org"
        },
        {
            "name": "Justin Gallardo",
            "email": "justin.gallardo@gmail.com"
        },
        {
            "name": "Chris Nehren",
            "email": "cnehren@pobox.com"
        },
        {
            "name": "Henri Niemeläinen",
            "email": "aivot-on@iki.fi"
        },
        {
            "name": "Alex Miles",
            "email": "ghostaldev@gmail.com"
        },
        {
            "name": "Simmo Saan",
            "email": "simmo.saan@gmail.com"
        }
    ],
    "dependencies": {
        "iconv": "~2.2.1",
        "irc-colors": "^1.1.0",
        "node-icu-charset-detector": "~0.2.0"
    },
    "description": "An IRC client library for node",
    "devDependencies": {
        "ansi-color": "0.2.1",
        "faucet": "0.0.1",
        "jscs": "1.9.0",
        "tape": "^3.0.3"
    },
    "directories": {},
    "dist": {
        "shasum": "3714f4768365a96d0b2f776bc91166beb2464bbc",
        "tarball": "https://registry.npmjs.org/irc/-/irc-0.5.2.tgz"
    },
    "engines": {
        "node": ">=0.10.0"
    },
    "gitHead": "be1084cbc91c452fe895f16613bd9718d8a7de12",
    "homepage": "https://github.com/martynsmith/node-irc#readme",
    "license": "GPL-3.0",
    "main": "lib/irc",
    "maintainers": [
        {
            "name": "martyn",
            "email": "martyn@dollyfish.net.nz"
        },
        {
            "name": "apeiron",
            "email": "cnehren+npm@pobox.com"
        },
        {
            "name": "jirwin",
            "email": "justin.gallardo@gmail.com"
        }
    ],
    "name": "irc",
    "optionalDependencies": {
        "iconv": "~2.2.1",
        "node-icu-charset-detector": "~0.2.0"
    },
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+ssh://git@github.com/martynsmith/node-irc.git"
    },
    "scripts": {
        "lint": "./node_modules/jscs/bin/jscs --preset=airbnb */*.js",
        "test": "./node_modules/faucet/bin/cmd.js test/test-*.js"
    },
    "version": "0.5.2"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module irc](#apidoc.module.irc)
1.  [function <span class="apidocSignatureSpan">irc.</span>Client (server, nick, opt)](#apidoc.element.irc.Client)
1.  [function <span class="apidocSignatureSpan">irc.</span>cycling_ping_timer (client)](#apidoc.element.irc.cycling_ping_timer)
1.  object <span class="apidocSignatureSpan">irc.</span>Client.prototype
1.  object <span class="apidocSignatureSpan">irc.</span>colors

#### [module irc.Client](#apidoc.module.irc.Client)
1.  [function <span class="apidocSignatureSpan">irc.</span>Client (server, nick, opt)](#apidoc.element.irc.Client.Client)
1.  [function <span class="apidocSignatureSpan">irc.Client.</span>super_ ()](#apidoc.element.irc.Client.super_)

#### [module irc.Client.prototype](#apidoc.module.irc.Client.prototype)
1.  [function <span class="apidocSignatureSpan">irc.Client.prototype.</span>_addWhoisData (nick, key, value, onlyIfExists)](#apidoc.element.irc.Client.prototype._addWhoisData)
1.  [function <span class="apidocSignatureSpan">irc.Client.prototype.</span>_clearWhoisData (nick)](#apidoc.element.irc.Client.prototype._clearWhoisData)
1.  [function <span class="apidocSignatureSpan">irc.Client.prototype.</span>_connectionHandler ()](#apidoc.element.irc.Client.prototype._connectionHandler)
1.  [function <span class="apidocSignatureSpan">irc.Client.prototype.</span>_handleCTCP (from, to, text, type, message)](#apidoc.element.irc.Client.prototype._handleCTCP)
1.  [function <span class="apidocSignatureSpan">irc.Client.prototype.</span>_speak (kind, target, text)](#apidoc.element.irc.Client.prototype._speak)
1.  [function <span class="apidocSignatureSpan">irc.Client.prototype.</span>_splitLongLines (words, maxLength, destination)](#apidoc.element.irc.Client.prototype._splitLongLines)
1.  [function <span class="apidocSignatureSpan">irc.Client.prototype.</span>_updateMaxLineLength ()](#apidoc.element.irc.Client.prototype._updateMaxLineLength)
1.  [function <span class="apidocSignatureSpan">irc.Client.prototype.</span>action (channel, text)](#apidoc.element.irc.Client.prototype.action)
1.  [function <span class="apidocSignatureSpan">irc.Client.prototype.</span>activateFloodProtection (interval)](#apidoc.element.irc.Client.prototype.activateFloodProtection)
1.  [function <span class="apidocSignatureSpan">irc.Client.prototype.</span>chanData (name, create)](#apidoc.element.irc.Client.prototype.chanData)
1.  [function <span class="apidocSignatureSpan">irc.Client.prototype.</span>connect (retryCount, callback)](#apidoc.element.irc.Client.prototype.connect)
1.  [function <span class="apidocSignatureSpan">irc.Client.prototype.</span>connectionTimedOut (conn)](#apidoc.element.irc.Client.prototype.connectionTimedOut)
1.  [function <span class="apidocSignatureSpan">irc.Client.prototype.</span>connectionWantsPing (conn)](#apidoc.element.irc.Client.prototype.connectionWantsPing)
1.  [function <span class="apidocSignatureSpan">irc.Client.prototype.</span>convertEncoding (str)](#apidoc.element.irc.Client.prototype.convertEncoding)
1.  [function <span class="apidocSignatureSpan">irc.Client.prototype.</span>ctcp (to, type, text)](#apidoc.element.irc.Client.prototype.ctcp)
1.  [function <span class="apidocSignatureSpan">irc.Client.prototype.</span>disconnect (message, callback)](#apidoc.element.irc.Client.prototype.disconnect)
1.  [function <span class="apidocSignatureSpan">irc.Client.prototype.</span>end ()](#apidoc.element.irc.Client.prototype.end)
1.  [function <span class="apidocSignatureSpan">irc.Client.prototype.</span>join (channel, callback)](#apidoc.element.irc.Client.prototype.join)
1.  [function <span class="apidocSignatureSpan">irc.Client.prototype.</span>list ()](#apidoc.element.irc.Client.prototype.list)
1.  [function <span class="apidocSignatureSpan">irc.Client.prototype.</span>notice (target, text)](#apidoc.element.irc.Client.prototype.notice)
1.  [function <span class="apidocSignatureSpan">irc.Client.prototype.</span>part (channel, message, callback)](#apidoc.element.irc.Client.prototype.part)
1.  [function <span class="apidocSignatureSpan">irc.Client.prototype.</span>say (target, text)](#apidoc.element.irc.Client.prototype.say)
1.  [function <span class="apidocSignatureSpan">irc.Client.prototype.</span>send (command)](#apidoc.element.irc.Client.prototype.send)
1.  [function <span class="apidocSignatureSpan">irc.Client.prototype.</span>whois (nick, callback)](#apidoc.element.irc.Client.prototype.whois)
1.  object <span class="apidocSignatureSpan">irc.Client.prototype.</span>_whoisData
1.  object <span class="apidocSignatureSpan">irc.Client.prototype.</span>chans
1.  object <span class="apidocSignatureSpan">irc.Client.prototype.</span>conn
1.  object <span class="apidocSignatureSpan">irc.Client.prototype.</span>modeForPrefix
1.  object <span class="apidocSignatureSpan">irc.Client.prototype.</span>prefixForMode

#### [module irc.colors](#apidoc.module.irc.colors)
1.  [function <span class="apidocSignatureSpan">irc.colors.</span>wrap (color, text, resetColor)](#apidoc.element.irc.colors.wrap)
1.  object <span class="apidocSignatureSpan">irc.colors.</span>codes

#### [module irc.cycling_ping_timer](#apidoc.module.irc.cycling_ping_timer)
1.  [function <span class="apidocSignatureSpan">irc.</span>cycling_ping_timer (client)](#apidoc.element.irc.cycling_ping_timer.cycling_ping_timer)
1.  [function <span class="apidocSignatureSpan">irc.cycling_ping_timer.</span>super_ ()](#apidoc.element.irc.cycling_ping_timer.super_)



# <a name="apidoc.module.irc"></a>[module irc](#apidoc.module.irc)

#### <a name="apidoc.element.irc.Client"></a>[function <span class="apidocSignatureSpan">irc.</span>Client (server, nick, opt)](#apidoc.element.irc.Client)
- description and source-code
```javascript
function Client(server, nick, opt) {
    var self = this;
    self.opt = {
        server: server,
        nick: nick,
        password: null,
        userName: 'nodebot',
        realName: 'nodeJS IRC client',
        port: 6667,
        localAddress: null,
        debug: false,
        showErrors: false,
        autoRejoin: false,
        autoConnect: true,
        channels: [],
        retryCount: null,
        retryDelay: 2000,
        secure: false,
        selfSigned: false,
        certExpired: false,
        floodProtection: false,
        floodProtectionDelay: 1000,
        sasl: false,
        stripColors: false,
        channelPrefixes: '&#',
        messageSplit: 512,
        encoding: false,
        webirc: {
          pass: '',
          ip: '',
          host: ''
        },
        millisecondsOfSilenceBeforePingSent: 15 * 1000,
        millisecondsBeforePingTimeout: 8 * 1000
    };

    // Features supported by the server
    // (initial values are RFC 1459 defaults. Zeros signify
    // no default or unlimited value)
    self.supported = {
        channel: {
            idlength: [],
            length: 200,
            limit: [],
            modes: { a: '', b: '', c: '', d: ''},
            types: self.opt.channelPrefixes
        },
        kicklength: 0,
        maxlist: [],
        maxtargets: [],
        modes: 3,
        nicklength: 9,
        topiclength: 0,
        usermodes: ''
    };

    if (typeof arguments[2] == 'object') {
        var keys = Object.keys(self.opt);
        for (var i = 0; i < keys.length; i++) {
            var k = keys[i];
            if (arguments[2][k] !== undefined)
                self.opt[k] = arguments[2][k];
        }
    }

    if (self.opt.floodProtection) {
        self.activateFloodProtection();
    }

    self.hostMask = '';

    // TODO - fail if nick or server missing
    // TODO - fail if username has a space in it
    if (self.opt.autoConnect === true) {
        self.connect();
    }

    self.addListener('raw', function(message) {
        var channels = [],
            channel,
            nick,
            from,
            text,
            to;

        switch (message.command) {
            case 'rpl_welcome':
                // Set nick to whatever the server decided it really is
                // (normally this is because you chose something too long and
                // the server has shortened it
                self.nick = message.args[0];
                // Note our hostmask to use it in splitting long messages.
                // We don't send our hostmask when issuing PRIVMSGs or NOTICEs,
                // of course, but rather the servers on the other side will
                // include it in messages and will truncate what we send if
                // the string is too long. Therefore, we need to be considerate
                // neighbors and truncate our messages accordingly.
                var welcomeStringWords = message.args[1].split(/\s+/);
                self.hostMask = welcomeStringWords[welcomeStringWords.length - 1];
                self._updateMaxLineLength();
                self.emit('registered', message);
                self.whois(self.nick, function(args) {
                    self.nick = args.nick;
                    self.hostMask = args.user + '@' + args.host;
                    self._updateMaxLineLength();
                });
                break;
            case 'rpl_myinfo':
                self.supported.usermodes = message.args[3];
                break;
            case 'rpl_isupport':
                message.args.forEach(function(arg) {
                    var match;
                    match = arg.match(/([A-Z]+)=(.*)/);
                    if (match) {
                        var param = match[1];
                        var value = match[2];
                        switch (param) {
                            case 'CHANLIMIT':
                                value.split(',').forEach(function(val) {
                                    val = val.split(':');
                                    self.supported ...
```
- example usage
```shell
...
## Basic Usage

This library provides basic IRC client functionality. In the simplest case you
can connect to an IRC server like so:

'''js
var irc = require('irc');
var client = new irc.Client('irc.yourserver.com', 'myNick', {
    channels: ['#channel'],
});
'''

Of course it's not much use once it's connected if that's all you have!

The client emits a large number of events that correlate to things you'd
...
```

#### <a name="apidoc.element.irc.cycling_ping_timer"></a>[function <span class="apidocSignatureSpan">irc.</span>cycling_ping_timer (client)](#apidoc.element.irc.cycling_ping_timer)
- description and source-code
```javascript
function CyclingPingTimer(client) {
    var timerNumber = ctr++;
    var started = false;
    var self = this;

    // Only one of these two should be non-null at any given time.
    var loopingTimeout = null;
    var pingWaitTimeout = null;

    // conditionally log debug messages
    function debug(msg) {
        if (client.opt.debug) {
            console.error('CyclingPingTimer ' + timerNumber + ': ' + msg);
        }
    }

    // set up EventEmitter functionality
    EventEmitter.call(self);

    self.on('wantPing', function() {
        debug('server silent for too long, let\'s send a PING');
        pingWaitTimeout = setTimeout(function() {
            self.stop();
            debug('ping timeout!');
            self.emit('pingTimeout');
        }, client.opt.millisecondsBeforePingTimeout);
    });

    self.notifyOfActivity = function() {
        if (started) {
            self.stop();
            self.start();
        }
    };

    self.stop = function() {
        if (!started) {
            return;
        }
        started = false;

        clearTimeout(loopingTimeout);
        clearTimeout(pingWaitTimeout);

        loopingTimeout = null;
        pingWaitTimeout = null;
    };

    self.start = function() {
        if (started) {
            debug('can\'t start, not stopped!');
            return;
        }
        started = true;

        loopingTimeout = setTimeout(function() {
            loopingTimeout = null;
            self.emit('wantPing');
        }, client.opt.millisecondsOfSilenceBeforePingSent);
    };
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.irc.Client"></a>[module irc.Client](#apidoc.module.irc.Client)

#### <a name="apidoc.element.irc.Client.Client"></a>[function <span class="apidocSignatureSpan">irc.</span>Client (server, nick, opt)](#apidoc.element.irc.Client.Client)
- description and source-code
```javascript
function Client(server, nick, opt) {
    var self = this;
    self.opt = {
        server: server,
        nick: nick,
        password: null,
        userName: 'nodebot',
        realName: 'nodeJS IRC client',
        port: 6667,
        localAddress: null,
        debug: false,
        showErrors: false,
        autoRejoin: false,
        autoConnect: true,
        channels: [],
        retryCount: null,
        retryDelay: 2000,
        secure: false,
        selfSigned: false,
        certExpired: false,
        floodProtection: false,
        floodProtectionDelay: 1000,
        sasl: false,
        stripColors: false,
        channelPrefixes: '&#',
        messageSplit: 512,
        encoding: false,
        webirc: {
          pass: '',
          ip: '',
          host: ''
        },
        millisecondsOfSilenceBeforePingSent: 15 * 1000,
        millisecondsBeforePingTimeout: 8 * 1000
    };

    // Features supported by the server
    // (initial values are RFC 1459 defaults. Zeros signify
    // no default or unlimited value)
    self.supported = {
        channel: {
            idlength: [],
            length: 200,
            limit: [],
            modes: { a: '', b: '', c: '', d: ''},
            types: self.opt.channelPrefixes
        },
        kicklength: 0,
        maxlist: [],
        maxtargets: [],
        modes: 3,
        nicklength: 9,
        topiclength: 0,
        usermodes: ''
    };

    if (typeof arguments[2] == 'object') {
        var keys = Object.keys(self.opt);
        for (var i = 0; i < keys.length; i++) {
            var k = keys[i];
            if (arguments[2][k] !== undefined)
                self.opt[k] = arguments[2][k];
        }
    }

    if (self.opt.floodProtection) {
        self.activateFloodProtection();
    }

    self.hostMask = '';

    // TODO - fail if nick or server missing
    // TODO - fail if username has a space in it
    if (self.opt.autoConnect === true) {
        self.connect();
    }

    self.addListener('raw', function(message) {
        var channels = [],
            channel,
            nick,
            from,
            text,
            to;

        switch (message.command) {
            case 'rpl_welcome':
                // Set nick to whatever the server decided it really is
                // (normally this is because you chose something too long and
                // the server has shortened it
                self.nick = message.args[0];
                // Note our hostmask to use it in splitting long messages.
                // We don't send our hostmask when issuing PRIVMSGs or NOTICEs,
                // of course, but rather the servers on the other side will
                // include it in messages and will truncate what we send if
                // the string is too long. Therefore, we need to be considerate
                // neighbors and truncate our messages accordingly.
                var welcomeStringWords = message.args[1].split(/\s+/);
                self.hostMask = welcomeStringWords[welcomeStringWords.length - 1];
                self._updateMaxLineLength();
                self.emit('registered', message);
                self.whois(self.nick, function(args) {
                    self.nick = args.nick;
                    self.hostMask = args.user + '@' + args.host;
                    self._updateMaxLineLength();
                });
                break;
            case 'rpl_myinfo':
                self.supported.usermodes = message.args[3];
                break;
            case 'rpl_isupport':
                message.args.forEach(function(arg) {
                    var match;
                    match = arg.match(/([A-Z]+)=(.*)/);
                    if (match) {
                        var param = match[1];
                        var value = match[2];
                        switch (param) {
                            case 'CHANLIMIT':
                                value.split(',').forEach(function(val) {
                                    val = val.split(':');
                                    self.supported ...
```
- example usage
```shell
...
## Basic Usage

This library provides basic IRC client functionality. In the simplest case you
can connect to an IRC server like so:

'''js
var irc = require('irc');
var client = new irc.Client('irc.yourserver.com', 'myNick', {
    channels: ['#channel'],
});
'''

Of course it's not much use once it's connected if that's all you have!

The client emits a large number of events that correlate to things you'd
...
```

#### <a name="apidoc.element.irc.Client.super_"></a>[function <span class="apidocSignatureSpan">irc.Client.</span>super_ ()](#apidoc.element.irc.Client.super_)
- description and source-code
```javascript
function EventEmitter() {
  EventEmitter.init.call(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.irc.Client.prototype"></a>[module irc.Client.prototype](#apidoc.module.irc.Client.prototype)

#### <a name="apidoc.element.irc.Client.prototype._addWhoisData"></a>[function <span class="apidocSignatureSpan">irc.Client.prototype.</span>_addWhoisData (nick, key, value, onlyIfExists)](#apidoc.element.irc.Client.prototype._addWhoisData)
- description and source-code
```javascript
_addWhoisData = function (nick, key, value, onlyIfExists) {
    if (onlyIfExists && !this._whoisData[nick]) return;
    this._whoisData[nick] = this._whoisData[nick] || {nick: nick};
    this._whoisData[nick][key] = value;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.irc.Client.prototype._clearWhoisData"></a>[function <span class="apidocSignatureSpan">irc.Client.prototype.</span>_clearWhoisData (nick)](#apidoc.element.irc.Client.prototype._clearWhoisData)
- description and source-code
```javascript
_clearWhoisData = function (nick) {
    // Ensure that at least the nick exists before trying to return
    this._addWhoisData(nick, 'nick', nick);
    var data = this._whoisData[nick];
    delete this._whoisData[nick];
    return data;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.irc.Client.prototype._connectionHandler"></a>[function <span class="apidocSignatureSpan">irc.Client.prototype.</span>_connectionHandler ()](#apidoc.element.irc.Client.prototype._connectionHandler)
- description and source-code
```javascript
_connectionHandler = function () {
    if (this.opt.webirc.ip && this.opt.webirc.pass && this.opt.webirc.host) {
        this.send('WEBIRC', this.opt.webirc.pass, this.opt.userName, this.opt.webirc.host, this.opt.webirc.ip);
    }
    if (this.opt.sasl) {
        // see http://ircv3.atheme.org/extensions/sasl-3.1
        this.send('CAP REQ', 'sasl');
    } else if (this.opt.password) {
        this.send('PASS', this.opt.password);
    }
    if (this.opt.debug)
        util.log('Sending irc NICK/USER');
    this.send('NICK', this.opt.nick);
    this.nick = this.opt.nick;
    this._updateMaxLineLength();
    this.send('USER', this.opt.userName, 8, '*', this.opt.realName);

    this.conn.cyclingPingTimer.start();

    this.emit('connect');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.irc.Client.prototype._handleCTCP"></a>[function <span class="apidocSignatureSpan">irc.Client.prototype.</span>_handleCTCP (from, to, text, type, message)](#apidoc.element.irc.Client.prototype._handleCTCP)
- description and source-code
```javascript
_handleCTCP = function (from, to, text, type, message) {
    text = text.slice(1);
    text = text.slice(0, text.indexOf('\u0001'));
    var parts = text.split(' ');
    this.emit('ctcp', from, to, text, type, message);
    this.emit('ctcp-' + type, from, to, text, message);
    if (type === 'privmsg' && text === 'VERSION')
        this.emit('ctcp-version', from, to, message);
    if (parts[0] === 'ACTION' && parts.length > 1)
        this.emit('action', from, to, parts.slice(1).join(' '), message);
    if (parts[0] === 'PING' && type === 'privmsg' && parts.length > 1)
        this.ctcp(from, 'notice', text);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.irc.Client.prototype._speak"></a>[function <span class="apidocSignatureSpan">irc.Client.prototype.</span>_speak (kind, target, text)](#apidoc.element.irc.Client.prototype._speak)
- description and source-code
```javascript
_speak = function (kind, target, text) {
    var self = this;
    var maxLength = Math.min(this.maxLineLength - target.length, this.opt.messageSplit);
    if (typeof text !== 'undefined') {
        text.toString().split(/\r?\n/).filter(function(line) {
            return line.length > 0;
        }).forEach(function(line) {
            var linesToSend = self._splitLongLines(line, maxLength, []);
            linesToSend.forEach(function(toSend) {
                self.send(kind, target, toSend);
                if (kind == 'PRIVMSG') {
                    self.emit('selfMessage', target, toSend);
                }
            });
        });
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.irc.Client.prototype._splitLongLines"></a>[function <span class="apidocSignatureSpan">irc.Client.prototype.</span>_splitLongLines (words, maxLength, destination)](#apidoc.element.irc.Client.prototype._splitLongLines)
- description and source-code
```javascript
_splitLongLines = function (words, maxLength, destination) {
    maxLength = maxLength || 450; // If maxLength hasn't been initialized yet, prefer an arbitrarily low line length over crashing
.
    if (words.length == 0) {
        return destination;
    }
    if (words.length <= maxLength) {
        destination.push(words);
        return destination;
    }
    var c = words[maxLength];
    var cutPos;
    var wsLength = 1;
    if (c.match(/\s/)) {
        cutPos = maxLength;
    } else {
        var offset = 1;
        while ((maxLength - offset) > 0) {
            var c = words[maxLength - offset];
            if (c.match(/\s/)) {
                cutPos = maxLength - offset;
                break;
            }
            offset++;
        }
        if (maxLength - offset <= 0) {
            cutPos = maxLength;
            wsLength = 0;
        }
    }
    var part = words.substring(0, cutPos);
    destination.push(part);
    return this._splitLongLines(words.substring(cutPos + wsLength, words.length), maxLength, destination);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.irc.Client.prototype._updateMaxLineLength"></a>[function <span class="apidocSignatureSpan">irc.Client.prototype.</span>_updateMaxLineLength ()](#apidoc.element.irc.Client.prototype._updateMaxLineLength)
- description and source-code
```javascript
_updateMaxLineLength = function () {
    // 497 = 510 - (":" + "!" + " PRIVMSG " + " :").length;
    // target is determined in _speak() and subtracted there
    this.maxLineLength = 497 - this.nick.length - this.hostMask.length;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.irc.Client.prototype.action"></a>[function <span class="apidocSignatureSpan">irc.Client.prototype.</span>action (channel, text)](#apidoc.element.irc.Client.prototype.action)
- description and source-code
```javascript
action = function (channel, text) {
    var self = this;
    if (typeof text !== 'undefined') {
        text.toString().split(/\r?\n/).filter(function(line) {
            return line.length > 0;
        }).forEach(function(line) {
            self.say(channel, '\u0001ACTION ' + line + '\u0001');
        });
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.irc.Client.prototype.activateFloodProtection"></a>[function <span class="apidocSignatureSpan">irc.Client.prototype.</span>activateFloodProtection (interval)](#apidoc.element.irc.Client.prototype.activateFloodProtection)
- description and source-code
```javascript
activateFloodProtection = function (interval) {

    var cmdQueue = [],
        safeInterval = interval || this.opt.floodProtectionDelay,
        self = this,
        origSend = this.send,
        dequeue;

    // Wrapper for the original function. Just put everything to on central
    // queue.
    this.send = function() {
        cmdQueue.push(arguments);
    };

    this._sendImmediate = function() {
        origSend.apply(self, arguments);
    };

    this._clearCmdQueue = function() {
        cmdQueue = [];
    };

    dequeue = function() {
        var args = cmdQueue.shift();
        if (args) {
            origSend.apply(self, args);
        }
    };

    // Slowly unpack the queue without flooding.
    setInterval(dequeue, safeInterval);
    dequeue();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.irc.Client.prototype.chanData"></a>[function <span class="apidocSignatureSpan">irc.Client.prototype.</span>chanData (name, create)](#apidoc.element.irc.Client.prototype.chanData)
- description and source-code
```javascript
chanData = function (name, create) {
    var key = name.toLowerCase();
    if (create) {
        this.chans[key] = this.chans[key] || {
            key: key,
            serverName: name,
            users: {},
            modeParams: {},
            mode: ''
        };
    }

    return this.chans[key];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.irc.Client.prototype.connect"></a>[function <span class="apidocSignatureSpan">irc.Client.prototype.</span>connect (retryCount, callback)](#apidoc.element.irc.Client.prototype.connect)
- description and source-code
```javascript
connect = function (retryCount, callback) {
    if (typeof (retryCount) === 'function') {
        callback = retryCount;
        retryCount = undefined;
    }
    retryCount = retryCount || 0;
    if (typeof (callback) === 'function') {
        this.once('registered', callback);
    }
    var self = this;
    self.chans = {};

    // socket opts
    var connectionOpts = {
        host: self.opt.server,
        port: self.opt.port
    };

    // local address to bind to
    if (self.opt.localAddress)
        connectionOpts.localAddress = self.opt.localAddress;

    // try to connect to the server
    if (self.opt.secure) {
        connectionOpts.rejectUnauthorized = !self.opt.selfSigned;

        if (typeof self.opt.secure == 'object') {
            // copy "secure" opts to options passed to connect()
            for (var f in self.opt.secure) {
                connectionOpts[f] = self.opt.secure[f];
            }
        }

        self.conn = tls.connect(connectionOpts, function() {
            // callback called only after successful socket connection
            self.conn.connected = true;
            if (self.conn.authorized ||
                (self.opt.selfSigned &&
                    (self.conn.authorizationError   === 'DEPTH_ZERO_SELF_SIGNED_CERT' ||
                     self.conn.authorizationError === 'UNABLE_TO_VERIFY_LEAF_SIGNATURE' ||
                     self.conn.authorizationError === 'SELF_SIGNED_CERT_IN_CHAIN')) ||
                (self.opt.certExpired &&
                 self.conn.authorizationError === 'CERT_HAS_EXPIRED')) {
                // authorization successful

                if (!self.opt.encoding) {
                    self.conn.setEncoding('utf-8');
                }

                if (self.opt.certExpired &&
                    self.conn.authorizationError === 'CERT_HAS_EXPIRED') {
                    util.log('Connecting to server with expired certificate');
                }

                self._connectionHandler();
            } else {
                // authorization failed
                util.log(self.conn.authorizationError);
            }
        });
    } else {
        self.conn = net.createConnection(connectionOpts, self._connectionHandler.bind(self));
    }
    self.conn.requestedDisconnect = false;
    self.conn.setTimeout(0);

    // Each connection gets its own CyclingPingTimer. The connection forwards the timer's 'timeout' and 'wantPing' events
    // to the client object via calling the connectionTimedOut() and connectionWantsPing() functions.
    //
    // Since the client's "current connection" value changes over time because of retry functionality,
    // the client should ignore timeout/wantPing events that come from old connections.
    self.conn.cyclingPingTimer = new CyclingPingTimer(self);
    (function(conn) {
        conn.cyclingPingTimer.on('pingTimeout', function() {
            self.connectionTimedOut(conn);
        });
        conn.cyclingPingTimer.on('wantPing', function() {
            self.connectionWantsPing(conn);
        });
    }(self.conn));

    if (!self.opt.encoding) {
        self.conn.setEncoding('utf8');
    }

    var buffer = new Buffer('');

    function handleData(chunk) {
        self.conn.cyclingPingTimer.notifyOfActivity();

        if (typeof (chunk) === 'string') {
            buffer += chunk;
        } else {
            buffer = Buffer.concat([buffer, chunk]);
        }

        var lines = self.convertEncoding(buffer).toString().split(lineDelimiter);

        if (lines.pop()) {
            // if buffer is not ended with \r\n, there's more chunks.
            return;
        } else {
            // else, initialize the buffer.
            buffer = new Buffer('');
        }

        lines.forEach(function iterator(line) {
            if (line.length) {
                var message = parseMessage(line, self.opt.stripColors);

                try {
                    self.emit('raw', message);
                } catch (err) {
                    if (!self.conn.requestedDisconnect) {
                        throw err;
                    } ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.irc.Client.prototype.connectionTimedOut"></a>[function <span class="apidocSignatureSpan">irc.Client.prototype.</span>connectionTimedOut (conn)](#apidoc.element.irc.Client.prototype.connectionTimedOut)
- description and source-code
```javascript
connectionTimedOut = function (conn) {
    var self = this;
    if (conn !== self.conn) {
        // Only care about a timeout event if it came from the connection
        // that is most current.
        return;
    }
    self.end();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.irc.Client.prototype.connectionWantsPing"></a>[function <span class="apidocSignatureSpan">irc.Client.prototype.</span>connectionWantsPing (conn)](#apidoc.element.irc.Client.prototype.connectionWantsPing)
- description and source-code
```javascript
connectionWantsPing = function (conn) {
    var self = this;
    if (conn !== self.conn) {
        // Only care about a wantPing event if it came from the connection
        // that is most current.
        return;
    }
    self.send('PING', (pingCounter++).toString());
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.irc.Client.prototype.convertEncoding"></a>[function <span class="apidocSignatureSpan">irc.Client.prototype.</span>convertEncoding (str)](#apidoc.element.irc.Client.prototype.convertEncoding)
- description and source-code
```javascript
convertEncoding = function (str) {
    var self = this, out = str;

    if (self.opt.encoding) {
        try {
            var charsetDetector = require('node-icu-charset-detector');
            var Iconv = require('iconv').Iconv;
            var charset = charsetDetector.detectCharset(str);
            var converter = new Iconv(charset.toString(), self.opt.encoding);

            out = converter.convert(str);
        } catch (err) {
            if (self.opt.debug) {
                util.log('\u001b[01;31mERROR: ' + err + '\u001b[0m');
                util.inspect({ str: str, charset: charset });
            }
        }
    }

    return out;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.irc.Client.prototype.ctcp"></a>[function <span class="apidocSignatureSpan">irc.Client.prototype.</span>ctcp (to, type, text)](#apidoc.element.irc.Client.prototype.ctcp)
- description and source-code
```javascript
ctcp = function (to, type, text) {
    return this[type === 'privmsg' ? 'say' : 'notice'](to, '\u0001' + text + '\u0001');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.irc.Client.prototype.disconnect"></a>[function <span class="apidocSignatureSpan">irc.Client.prototype.</span>disconnect (message, callback)](#apidoc.element.irc.Client.prototype.disconnect)
- description and source-code
```javascript
disconnect = function (message, callback) {
    if (typeof (message) === 'function') {
        callback = message;
        message = undefined;
    }
    message = message || 'node-irc says goodbye';
    var self = this;
    if (self.conn.readyState == 'open') {
        var sendFunction;
        if (self.opt.floodProtection) {
            sendFunction = self._sendImmediate;
            self._clearCmdQueue();
        } else {
            sendFunction = self.send;
        }
        sendFunction.call(self, 'QUIT', message);
    }
    self.conn.requestedDisconnect = true;
    if (typeof (callback) === 'function') {
        self.conn.once('end', callback);
    }
    self.conn.end();
}
```
- example usage
```shell
...
repl.context.repl = repl;
repl.context.util = util;
repl.context.irc = irc;
repl.context.c = c;

repl.inputStream.addListener('close', function() {
    console.log("\nClosing session");
    c.disconnect('Closing session');
});
...
```

#### <a name="apidoc.element.irc.Client.prototype.end"></a>[function <span class="apidocSignatureSpan">irc.Client.prototype.</span>end ()](#apidoc.element.irc.Client.prototype.end)
- description and source-code
```javascript
end = function () {
    if (this.conn) {
        this.conn.cyclingPingTimer.stop();
        this.conn.destroy();
    }
    this.conn = null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.irc.Client.prototype.join"></a>[function <span class="apidocSignatureSpan">irc.Client.prototype.</span>join (channel, callback)](#apidoc.element.irc.Client.prototype.join)
- description and source-code
```javascript
join = function (channel, callback) {
    var channelName =  channel.split(' ')[0];
    this.once('join' + channelName, function() {
        // if join is successful, add this channel to opts.channels
        // so that it will be re-joined upon reconnect (as channels
        // specified in options are)
        if (this.opt.channels.indexOf(channel) == -1) {
            this.opt.channels.push(channel);
        }

        if (typeof (callback) == 'function') {
            return callback.apply(this, arguments);
        }
    });
    this.send.apply(this, ['JOIN'].concat(channel.split(' ')));
}
```
- example usage
```shell
...
    console.log(from + ' => #yourchannel: ' + message);
});
'''

At the moment there are functions for joining:

'''js
client.join('#yourchannel yourpass');
'''

parting:

'''js
client.part('#yourchannel');
'''
...
```

#### <a name="apidoc.element.irc.Client.prototype.list"></a>[function <span class="apidocSignatureSpan">irc.Client.prototype.</span>list ()](#apidoc.element.irc.Client.prototype.list)
- description and source-code
```javascript
list = function () {
    var args = Array.prototype.slice.call(arguments, 0);
    args.unshift('LIST');
    this.send.apply(this, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.irc.Client.prototype.notice"></a>[function <span class="apidocSignatureSpan">irc.Client.prototype.</span>notice (target, text)](#apidoc.element.irc.Client.prototype.notice)
- description and source-code
```javascript
notice = function (target, text) {
    this._speak('NOTICE', target, text);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.irc.Client.prototype.part"></a>[function <span class="apidocSignatureSpan">irc.Client.prototype.</span>part (channel, message, callback)](#apidoc.element.irc.Client.prototype.part)
- description and source-code
```javascript
part = function (channel, message, callback) {
    if (typeof (message) === 'function') {
        callback = message;
        message = undefined;
    }
    if (typeof (callback) == 'function') {
        this.once('part' + channel, callback);
    }

    // remove this channel from this.opt.channels so we won't rejoin
    // upon reconnect
    if (this.opt.channels.indexOf(channel) != -1) {
        this.opt.channels.splice(this.opt.channels.indexOf(channel), 1);
    }

    if (message) {
        this.send('PART', channel, message);
    } else {
        this.send('PART', channel);
    }
}
```
- example usage
```shell
...
'''js
client.join('#yourchannel yourpass');
'''

parting:

'''js
client.part('#yourchannel');
'''

talking:

'''js
client.say('#yourchannel', "I'm a bot!");
client.say('nonbeliever', "SRSLY, I AM!");
...
```

#### <a name="apidoc.element.irc.Client.prototype.say"></a>[function <span class="apidocSignatureSpan">irc.Client.prototype.</span>say (target, text)](#apidoc.element.irc.Client.prototype.say)
- description and source-code
```javascript
say = function (target, text) {
    this._speak('PRIVMSG', target, text);
}
```
- example usage
```shell
...
'''js
client.part('#yourchannel');
'''

talking:

'''js
client.say('#yourchannel', "I'm a bot!");
client.say('nonbeliever', "SRSLY, I AM!");
'''

and many others. Check out the API documentation for a complete reference.

For any commands that there aren't methods for you can use the send() method
which sends raw messages to the server:
...
```

#### <a name="apidoc.element.irc.Client.prototype.send"></a>[function <span class="apidocSignatureSpan">irc.Client.prototype.</span>send (command)](#apidoc.element.irc.Client.prototype.send)
- description and source-code
```javascript
send = function (command) {
    var args = Array.prototype.slice.call(arguments);

    // Note that the command arg is included in the args array as the first element

    if (args[args.length - 1].match(/\s/) || args[args.length - 1].match(/^:/) || args[args.length - 1] === '') {
        args[args.length - 1] = ':' + args[args.length - 1];
    }

    if (this.opt.debug)
        util.log('SEND: ' + args.join(' '));

    if (!this.conn.requestedDisconnect) {
        this.conn.write(args.join(' ') + '\r\n');
    }
}
```
- example usage
```shell
...

and many others. Check out the API documentation for a complete reference.

For any commands that there aren't methods for you can use the send() method
which sends raw messages to the server:

'''js
client.send('MODE', '#yourchannel', '+o', 'yournick');
'''

## Help! - it keeps crashing!

When the client receives errors from the IRC network, it emits an "error"
event. As stated in the [Node JS EventEmitter documentation](http://nodejs.org/api/events.html#events_class_events_eventemitter)
if you don't bind
something to this error, it will cause a fatal stack trace.
...
```

#### <a name="apidoc.element.irc.Client.prototype.whois"></a>[function <span class="apidocSignatureSpan">irc.Client.prototype.</span>whois (nick, callback)](#apidoc.element.irc.Client.prototype.whois)
- description and source-code
```javascript
whois = function (nick, callback) {
    if (typeof callback === 'function') {
        var callbackWrapper = function(info) {
            if (info.nick.toLowerCase() == nick.toLowerCase()) {
                this.removeListener('whois', callbackWrapper);
                return callback.apply(this, arguments);
            }
        };
        this.addListener('whois', callbackWrapper);
    }
    this.send('WHOIS', nick);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.irc.colors"></a>[module irc.colors](#apidoc.module.irc.colors)

#### <a name="apidoc.element.irc.colors.wrap"></a>[function <span class="apidocSignatureSpan">irc.colors.</span>wrap (color, text, resetColor)](#apidoc.element.irc.colors.wrap)
- description and source-code
```javascript
function wrap(color, text, resetColor) {
    if (codes[color]) {
        text = codes[color] + text;
        text += (codes[resetColor]) ? codes[resetColor] : codes.reset;
    }
    return text;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.irc.cycling_ping_timer"></a>[module irc.cycling_ping_timer](#apidoc.module.irc.cycling_ping_timer)

#### <a name="apidoc.element.irc.cycling_ping_timer.cycling_ping_timer"></a>[function <span class="apidocSignatureSpan">irc.</span>cycling_ping_timer (client)](#apidoc.element.irc.cycling_ping_timer.cycling_ping_timer)
- description and source-code
```javascript
function CyclingPingTimer(client) {
    var timerNumber = ctr++;
    var started = false;
    var self = this;

    // Only one of these two should be non-null at any given time.
    var loopingTimeout = null;
    var pingWaitTimeout = null;

    // conditionally log debug messages
    function debug(msg) {
        if (client.opt.debug) {
            console.error('CyclingPingTimer ' + timerNumber + ': ' + msg);
        }
    }

    // set up EventEmitter functionality
    EventEmitter.call(self);

    self.on('wantPing', function() {
        debug('server silent for too long, let\'s send a PING');
        pingWaitTimeout = setTimeout(function() {
            self.stop();
            debug('ping timeout!');
            self.emit('pingTimeout');
        }, client.opt.millisecondsBeforePingTimeout);
    });

    self.notifyOfActivity = function() {
        if (started) {
            self.stop();
            self.start();
        }
    };

    self.stop = function() {
        if (!started) {
            return;
        }
        started = false;

        clearTimeout(loopingTimeout);
        clearTimeout(pingWaitTimeout);

        loopingTimeout = null;
        pingWaitTimeout = null;
    };

    self.start = function() {
        if (started) {
            debug('can\'t start, not stopped!');
            return;
        }
        started = true;

        loopingTimeout = setTimeout(function() {
            loopingTimeout = null;
            self.emit('wantPing');
        }, client.opt.millisecondsOfSilenceBeforePingSent);
    };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.irc.cycling_ping_timer.super_"></a>[function <span class="apidocSignatureSpan">irc.cycling_ping_timer.</span>super_ ()](#apidoc.element.irc.cycling_ping_timer.super_)
- description and source-code
```javascript
function EventEmitter() {
  EventEmitter.init.call(this);
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
