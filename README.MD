
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

Copyright (c) 2016, LogRhythm
All rights reserved.

Redistribution and use in source and binary forms, with or without
modification, are permitted provided that the following conditions are met:
* Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
* Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
* Neither the name of LogRhythm, LogRhythm Labs, nor the names of any of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.

