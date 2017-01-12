
        LogRhythm Security Operations
        Twilio SMS Notification SmartResponse
        greg . foss [at] logrhythm . com
        v0.1 -- April 2016

## [About]

Blog Post => <a href="https://logrhythm.com/blog/sms-alerting-via-smartresponse/?utm_source=github">https://logrhythm.com/blog/sms-alerting-via-smartresponse/</a>

Automate SMS alerting from the SIEM via <a href="https://www.twilio.com/">Twilio</a> SMS messaging integration.


## [How To]

 	PS C:\> .\twilio-sms.ps1 -from_number [number] -to_number [number] -account_sid [sid] -auth_token [token] -message "Test Message"
        This will send a basic SMS message

    You can also hard-code these attributes if you'd like to run this manually
        if you do, ensure that you remove the code signing key


## [Parameter Breakdown]

	-from_number    :    Defines the number to send the SMS from
    -to_number      :    Defines the number that SMS messages should be sent to
    -account_sid    :    Twilio Account SID
    -auth_token     :    Twilio Authentication Token
    -message        :    The SMS message text to send to the desired phone number.


## [License]

Copyright (c) 2016 LogRhythm

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

