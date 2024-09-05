# Hopsium Mod

## Briefing
Hopsium Mod is a disk encryption solution based on TrueCrypt 7.1, used in some Arccer games.

Encryption is at partition level. Encrypted partition will have a header `Hopsium Mod Boot Loader` at the beginning. With a damaged boot loader, the system will show a message as `Loader damaged! Use Rescue Disk: Repair Options > Restor Hopsium Mod Boot Loader`, essentially the same as an encrypted disk with a damaged TrueCrypt/VeraCrypt bootloader with a different name.

By booting from an encrypted partition, it will decrypt itself on-the-fly on boot and continue to boot from the inner PBR contained in it. Encrypted partitions could boot from any machine with a valid MBR on the disk, as decryption key is self contained and requires no external input to provide the key.

As vulnerabilities found in TrueCrypt, the master key could be extracted from the RAM image dump/DMA (though this is rendered hard as board used in many games have no PCIE slots for off-the-shelf DMA modules) from a virtual or physical machine , which could be used to decrypt the partition without the need for actual decryption key. Decrypting the disk doesn't require a valid bootloader.

## Keys
**Do not commit plain text keys to this section. Such PRs won't be accepted. As some of the games are still online and actively maintained, publishing keys in plain text could cause severe security risks to these games.**

If you managed to extract the keys, these information could be used to validate your keys. Notice these keys aren't guranteed to be used universally in all games.
<table>
<tr><td>HighPraise Series</td></tr>
<tr>
    <td rowspan=5>TrueCrypt Master Key</td>
</tr>
<tr>
    <td>CRC32</td><td>260A90C9</td>
</tr>
<tr>
    <td>SHA-256</td><td>9e40066cc75fb3cc85f855c2d18fd5ba36162714243e57ecf4c3aca985112adc</td>
</tr>
<tr>
    <td>SHA-1</td><td>23a7f3795324908f32ffb998668360b1d44b4da1<td>
</tr>
<tr>
    <td>MD5</td><td>cb5487e456ace65509eb9a9263d98443<td>
</tr>
</table>