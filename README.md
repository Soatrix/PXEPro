"This is the APT repo." 

To add the PXE Pro repository to your repos please run this command:
`echo "deb [trusted=yes] https://soatrix.github.io/PXEPro stable main" | sudo tee /etc/apt/sources.list.d/pxepro.list`

Then you can run:
```
sudo apt update
sudo apt install pxepro-snapshot    # or pxepro-enterprise depending on the branch
```
