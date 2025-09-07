# CLI Cheat Sheet  

This cheat sheet provides a quick comparison of commonly used commands across **Linux/macOS (Bash)**, **Windows CMD**, and **PowerShell**.  

---

## 🛠 General Commands  

| Task | Linux / macOS (Bash) | Windows CMD | PowerShell |
|------|-----------------------|-------------|------------|
| Show current user | `whoami` | `whoami` | `whoami` |
| Show current directory | `pwd` | `cd` | `Get-Location` |
| Show environment variables | `echo $VAR` | `set` | `$env:VAR` |
| Show system info | `uname -a` | `systeminfo` | `Get-ComputerInfo` |
| Show help for command | `man command` | `command /?` | `Get-Help command` |
| Echo text | `echo "Hello"` | `echo Hello` | `Write-Output "Hello"` |

---

## 📂 File System & File Operations  

| Task | Linux / macOS (Bash) | Windows CMD | PowerShell |
|------|-----------------------|-------------|------------|
| List files | `ls -la` | `dir` | `Get-ChildItem` |
| Change directory | `cd folder` | `cd folder` | `Set-Location folder` |
| Print working directory | `pwd` | `cd` | `Get-Location` |
| Create directory | `mkdir folder` | `mkdir folder` | `New-Item -ItemType Directory folder` |
| Create empty file | `touch file.txt` | `type nul > file.txt` | `New-Item file.txt` |
| Copy file | `cp file1 file2` | `copy file1 file2` | `Copy-Item file1 file2` |
| Move/Rename file | `mv old new` | `move old new` | `Move-Item old new` |
| Delete file | `rm file.txt` | `del file.txt` | `Remove-Item file.txt` |
| Delete directory | `rm -r folder` | `rmdir /s folder` | `Remove-Item folder -Recurse` |
| View file contents | `cat file.txt` | `type file.txt` | `Get-Content file.txt` |
| Search text in file | `grep "text" file.txt` | `find "text" file.txt` | `Select-String "text" file.txt` |
| Check file type | `file file.txt` | N/A | `Get-Item file.txt \| Format-List` |
| Download file | `wget url` | N/A | `Invoke-WebRequest url -OutFile file.txt` |

---

## 🌐 Networking & Troubleshooting  

| Task | Linux / macOS (Bash) | Windows CMD | PowerShell |
|------|-----------------------|-------------|------------|
| Show IP info | `ifconfig` / `ip addr` | `ipconfig` | `Get-NetIPAddress` |
| Test connectivity | `ping host` | `ping host` | `Test-Connection host` |
| Trace route | `traceroute host` | `tracert host` | `Test-NetConnection -TraceRoute host` |
| Show active connections | `netstat -tulnp` | `netstat -ano` | `Get-NetTCPConnection` |
| DNS lookup | `nslookup domain` | `nslookup domain` | `Resolve-DnsName domain` |
| SSH remote login | `ssh user@host` | N/A | `ssh user@host` |
| Copy over SSH | `scp file user@host:/path` | N/A | `scp file user@host:/path` |

---

## ⚙️ Processes & System Management  

| Task | Linux / macOS (Bash) | Windows CMD | PowerShell |
|------|-----------------------|-------------|------------|
| Show processes | `ps aux` | `tasklist` | `Get-Process` |
| Kill process | `kill PID` | `taskkill /PID 1234` | `Stop-Process -Id 1234` |
| Service management | `systemctl start nginx` | `net start servicename` | `Start-Service servicename` |
| Stop service | `systemctl stop nginx` | `net stop servicename` | `Stop-Service servicename` |
| Scheduled tasks | `crontab -e` | `schtasks` | `Get-ScheduledTask` |

---

## 🗃️ Filter & Sort

| Task | Linux / macOS (Bash) | Windows CMD | PowerShell |
|------|-----------------------|-------------|------------|
| filter objects based on specified conditions | ?? | ?? | Where-Object |
| sort objects based on specified properties | ?? | ?? | Sort-Object |


---

## 🔀 Operators (Linux only)  

| Operator | Description | Example Input | Example Output |
|----------|-------------|---------------|----------------|
| `&` | Run in background | `sleep 60 &` | Background job ID |
| `&&` | Run if previous succeeds | `mkdir test && cd test` | — |
| `>` | Redirect output (overwrite) | `echo hey > file.txt` | file.txt has `hey` |
| `>>` | Redirect output (append) | `echo you >> file.txt` | file.txt has `hey you` |

---
