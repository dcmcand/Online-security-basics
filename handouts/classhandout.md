## 1. Do your updates
Do your updates! As software companies learn about vulnerabilities, they send out fixes. By not doing updates, you are making an attackers job easy by letting them use known exploits against you. Any software that is on your computer needs to be kept up to date. For example:
* Your operating system.
  * For windows, use windows update. You can go to <http://windows.microsoft.com/en-us/windows/windows-update for more information>
  * For a Mac, you can access updates through the app store. For more information go to <https://support.apple.com/en-us/HT201541>
* Java - <https://www.java.com/en/download/help/java_update.xml>
* Flash - <https://helpx.adobe.com/flash-player.html>
* Antivirus - If your antivirus isn't up to date, it can't find all of the viruses out there.
* Web browsers - These directly interact with the internet and must be kept up to date.

This isn't a complete list by any means. Every piece of software on your computer needs to be kept up to date or it may turn into an exploitable vulnerability. By using a applications auto-update features, you get the protection without the effort.
## 2. If you can remember all of your passwords, you are doing it wrong
Passwords are absolutely essential to good computer security.  Using weak passwords and reusing passwords are some of the most common mistakes that people make.  Unfortunately, these mistakes make any potential breach, such as hacking someone's email, much more serious.  If you reuse passwords then getting your password for one thing often means they have your password for a lot of other things too. Hackers will use what is known as a credential stuffing attack to increase the impact of a breach. This means they will take compromised credentials and try them on a lot of websites automatically to see if they work other places. This means, if a website does have a breach you need to change the password on any other accounts that use the same password. It is far better to just not reuse passwords.

The best way to do this is to use a password manager. These programs will securely store your passwords for you. This means you only have one password to remember, the master password for your password manager. All the other passwords, you can forget about. This allows you to make them all very strong and unique without having to worry. Most password managers will also generate secure passwords for you. Some good ones are:
* LastPass - <https://www.lastpass.com>
* KeePass - <https://keepass.info>
* 1Password - <https://1password.com>
* Bitwarden - <https://bitwarden.com>

All of these password managers have a free level that you can try to get started. Even their premium levels are very affordable.

## 3. A Long Password is a Strong Password
The most important thing you can do to make a good password is make it long. As password length increases its strength goes up exponentially. If you simply increase the complexity, strength only increases linearly.

So if your password is **kdiosn** there are 26<sup>6</sup> or 308,915,776 possibilities.

If you increase the complexity by adding upper and lower case letters so your password is **KdIOsn** there are 52<sup>6</sup> or 18,770,609,664 possibilities.

On the other hand if you double the length instead of the complexity, and make the password **kdiosnplanew** then there are 26<sup>12</sup> or 94,289,566,600,000,000 possibilities. That is 4,826,809 times stronger that **KdIOsn**.

This assumes a random password that is not subject to a dictionary attack. A dictionary attack is where attackers have huge lists of commonly used passwords. Use your password manager to generate random passwords that are 16 digits long (or longer) and you will be very secure from someone guessing your password.

For your master password, this unfortunately won't work. There are two methods to deal with this.

1. Use the first letter of every word in a phrase. For example, "To be or not to be that is the question" becomes **tbontbtitq**. It is hard to get a really long password like this, and it could possibly be subject to a dictionary attack if you use a very common phrase, but it is decently strong and easily remembered.
2. Use a passphrase. This takes a string of four or five **unrelated** words to make a passphrase. A classic example is [Correct Horse Battery Staple](https://www.xkcd.com/936/). For added complexity, you can change the seperator to something other than a space (yes spaces are valid to use in a password) **Correct%Horse%Battery%Staple**, change or alternate the case **CORRECT%horse%BATTERY%staple** or add padding digits at the beginning and end **26CORRECT%horse%BATTERY%staple52**. The key is that we are good at remembering strings of words, but they are still difficult for computers to brute force. As long as you are actually using random words, this is a very secure method. For help choosing a random passphrase, check out [diceware](http://world.std.com/%7Ereinhold/diceware.html). Remember, if you are using a password generator, you should only need to remember one password.

## 4. Don't rely on passwords
When authenticating your identity (which is really what passwords are all about) there are a number of ways (factors) that can be used.  You can rely on something you know (a password, pin number, secret question, etc), something you have (texting a code to your cell phone or emailing you a code, requiring a hardware key such as a yubikey, etc) or something you are (facial recognition, thumbprint, etc).  Most account use passwords as a single factor for authentication.  However, many sites are now moving to using two factor authentication.  This typically means texting you a code when you try to sign in, or in the case of google, having a smart phone app that generates codes that are needed to login.  This ensures that even if someone steals your password, they can't get into your account without also having your cell phone.

Advantages:

  1. Extremely secure
  2. Normally very convenient

Disadvantages:

  1. Many sites don't support two factor authentication
  2. Normally requires a smart phone although there are other types of two factor authentication

If it is available, two factor authentication is by far the best and most secure way to set up your accounts
##  5. If you don't back it up, you don't care about it
Backups protect important information against malicious acts (such as ransomware), accidents (hard drive dies or computer is lost), and disasters (home burns down). The 3-2-1 ensures that your backups are protected against all of these. Backup anything that you can’t be easily replaced on your computer.

**3** copies of your data ensures redunancy. A virus or hardware failure won’t wipe out your data.

**2** different types of media means you aren’t storing both copies on the same hard drive. Having one copy on your computer and one copy on an external hard drive or thumb drive means that your computer dying or getting stolen won’t mean you lose everything.

**1** copy offsite protects against disasters such as your house burning down or getting flooded. One copy being physically separated means you have a safe copy regardless. Cloud backups are a popular way to get an offsite backup.

Compare Cloud backup software at: <https://en.wikipedia.org/wiki/Comparison_of_online_backup_services>

## 6. Backups are worthless, restores are priceless
In February 2017, [Gitlab](https://gitlab.com) lost six hours worth of customer data. They had multiple backup systems in place, yet all of them failed because they weren't properly tested and monitored. The only reason that they didn't lose more data is that an engineer working there had made a manual backup earlier in the day.

Backups can fail for a number of reasons. Regularly checking that you can restore files from your backups means that when you need your backups, they won't fail you.
## 7. Send letters, not postcards
When you send unencrypted traffic on the internet, it is like sending a postcard. Anyone along the path can read it. By using end to end encryption, you make sure that only the people that you want to read your message can do so. This is a feature that you should look for with any type of internet connected traffic you send.

The most common internet traffic is http traffic. This is how your web browser loads websites. When you check your email, go to your bank, buy something on Amazon, or look at cute kitty pictures, it is done over http. However, http has no encryption built in. To address that, a more secure protocol was created that is called https. These days, all websites should be using https. It provides end to end encryption. Like sending a letter, observers can see where the traffic is going, but can't read the message. In more technical terms, https does not protect metadata, but does protect content. This means an observer can see that you are going to https://mybank.com, but won't be able to see any of your traffic like your password or account number. They can see you are going to https://webmd.com, but can't see what condition you are looking up. Any traffic you send that isn't protected by http can be seen by anybody in the traffic's route.

This applies to messaging as well. Texting using sms is very convenient, but provides no security at all. Apps such as iMessage and WhatsApp provide more security. If you really want to chat securely, use [Signal](https://www.signal.org/). This provides strong end to end encryption and is very secure. It is as easy to use as normal text messaging, but prevents any snooping on your messages. You can even set your messages to autodestruct after a set length of time if you want to.

## 8. Practice defensive browsing
The internet is full of people who want to profit off of you. The most benign of these simply want to show you ads, but many want to collect huge amounts of data on you, follow you from website to website, or even infect your computer with malware. We are still in the wild west stage of the internet, and you would do well to have a defensive mindset when browsing (or reading emails). There are some things that you can do to help your privacy and security.

You can increase your security and privacy by using these browser plugins.
1. **uBlock Origin** - this ad blocker is very effective and light weight. It can be easily customized or disabled if you need to. It is available for [chrome](https://chrome.google.com/webstore/detail/ublock-origin/cjpalhdlnbpafiamejdnhcphjbkeiagm) and for [firefox](https://addons.mozilla.org/en-US/firefox/addon/ublock-origin/). Using a good ad blocker will reduce your vulnerability to malvertising (serving malware through ads) and save a good chunk of bandwidth, making sites load faster.
2. **HTTPS Everywhere** - this plugin forces sites to use an HTTPS version if one is available. It is put out by the Electronic Frontier Foundation. As discussed earlier, HTTPS is very important for maintaining your privacy and security online. It is available at <https://www.eff.org/https-everywhere> for Firefox, Chrome, and Opera.
3. **Privacy Badger** - Also from the EFF, privacy badger prevents online tracking. Many websites attempt to track your web browsing across many sites. Privacy badger blocks these trackers to keep companies from knowing about your browsing habits.


## 9. Don't trust public wifi

## 10. Don't trust email
