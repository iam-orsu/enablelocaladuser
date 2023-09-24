# enablelocaladuser
Get-LocalUser -Name "Administrator" | Enable-LocalUser
$UserAccount = Get-LocalUser -Name "Administrator"
$UserAccountPassword = "PutYourPasswordYouWantHere" | ConvertTo-SecureString -asPlainText -Force
$UserAccount | Set-LocalUser -Password $UserAccountPassword
