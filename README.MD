
        LogRhythm Security Operations
        Twilio SMS Notification SmartResponse
        greg . foss [at] logrhythm . com
        v0.1 -- April 2016

## [About]

Blog Post => Coming soon...

PSRecon gathers data from a remote Windows host using PowerShell (v2 or later), organizes the data into folders, hashes all extracted data, hashes PowerShell and various system properties, and sends the data off to the security team. The data can be pushed to a share, sent over email, or retained locally.

![email](/images/email-notification.png)

One nice part about the report is that everything is self-contained, making it easy to share as there is no reliance on a centralize server. Even the images are encoded directly into the report's HTML.

![reporting](/images/report-images.png)

This script also includes endpoint lockdown functionality. This can be useful when working through a malware outbreak incident, especially when there is risk that the malware will spread to a share or other critical systems within the enterprise. Sometimes the quickest and most effective way to stop the spread of malware is to simply knock the host offline until IT/Security can respond, following the extraction of forensic data. Alternatively to quarantining the host, PSRecon allows you to disable an active directory account as well.

Ideally, this script should be integrated with the organization's Active Defense frameworks to automate rapid forensic data acquisition and lock down the endpoint.

## [How To]

#####Run Twilio-SMS on local host:

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

