# PPJSON
Password-Protected JSON File Format

## Purpose
1. Allow for standard encryption of files
1. Using AES-256-GCM for symmetric encryption
1. Allow for metadata in plain text to provide important data to construct file 
1. For use with IPFS, where all files are in plaintext by default 

## Format Standard:
``
{
 "info": "Learn how to decrypt @ https://github.com/themaxsmith/PPJSON - [Any message to be read in plaintext]",
 "version": "1",
 "name": "[file name]",
 "type":"application/pdf",
 "payload": "[File contents in base64 string and then encrypted using AES-256-GCM]"
}
``
