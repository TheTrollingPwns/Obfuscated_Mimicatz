# Obfuscated_Mimicatz
- A few obfuscated mimicatz attempts. Going for glory. 


# V1
## Notes
- V1 was built using instructions from this link: https://medium.com/@markmotig/how-to-run-mimikatz-on-sharphellsgate-5<3b1eecccffe>
- Instructions were followed almost perfectly, except I used more up to date versions since some of the build artifacts required had newer versions released. I used what ever was newest as of 1.6.22, with the exception of the pe_to_shellcode exe's, those are all from the 0.8 release (as seen in the medium article). 
- Final build of executable is located at \Obfuscated_Mimicatz\V1\SharpHellsGate\SharpHellsGate\bin\Release\net5.0\SharpHellsGate.exe 
## Results
- I get an error message | `Error ntdll!NtWaitForSingleObject (0x258x8)` | when the program first, launches but it does not seem to be fatal, because I can just hit the return key a few times and then get a mimikatz shell.
	- Overall, I think it works! Could be sneakier though... Would benefit from removing the static strings that reference "HellsGate" and also possibly custom compiling mimikatz. Maybe I will try to do that later...

	