# NewDire
Func _AddDllDirectory($sNewDirectory)     $aRet = DllCall("Kernel32.dll", "ptr", "AddDllDirectory", "wstr", $sNewDirectory)     If @error Then Return SetError(@error, 0, 0)     Return $aRet[0] EndFunc
