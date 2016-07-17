# virtualhost-ftp

Usage:

    sudo bash create-project [OPTIONS] [HOSTNAME]   
    [OPTIONS]                                          
        -c,  -create      Create a new Web Application. 
        -s,  -sslhost     Create vhost with https.
        -f,  -cftp        Create FTP Account.  
        -e,  -enable      Enable disabled Web Application.
        -d,  -disable     Disable existing Web Application.
        -u,  -uhost       Update Existing Applications.
        -us, -usslhost    Update Existing SSL Application.
        -p,  -upass       Update Existing FTP account Password.
        -r,  -remove      Delele existing Web Application.
        -cl, -clone       Clone git/svn Repo to Application.
        -up, -repoUpdate  Update Existing Repo
        -ht, -htaccess    Create .htaccess file
        -h,  -help        Help, Usage       
        
    [HOSTNAME]                                          
        Eg:                                            
            example.com                               
            www.example.com   
            
    Examples:
        sudo bash create-project -cl www.example.com 
        sudo bash create-project -ur www.example.com 
        sudo bash create-project -c www.example.com 
        sudo bash create-project -remove www.example.com 
        
    For SSL Key Chain :                                
        Create directory under the 'cert' directory with the name of host,
        and upload all the SSL Certificate Files to the respective directory.  
        Eg :
            cert/www.example.com/example-ssl.crt
            cert/www.example.com/example-ssl.pem
            cert/www.example.com/ca-bundle.crl
            
    --
    author Rolind Roy <rolind.roy@gmail.com>
