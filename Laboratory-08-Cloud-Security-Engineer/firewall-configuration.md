- The command used to allow SSH. 
`sudo ufw allow ssh`

- The commands used to set the Default Deny policy. 
`sudo ufw default deny incoming`
`sudo ufw default allow outgoing `

- The command used to allow Port 8080. 
`sudo ufw allow 8080/tcp `

- A brief 1-sentence explanation of what would happen if you ran sudo ufw enable  before running sudo ufw allow ssh.
When you run `sudo ufw enable ` before running the sudo ufw allow ssh you will lockout yourserlf into your own container server.
