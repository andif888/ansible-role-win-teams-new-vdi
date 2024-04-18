# ansible-role-win-teams-new-vdi

Role to install Microsoft Teams (new) on Windows VDI

## Table of content

- [Requirements](#requirements)
- [Default Variables](#default-variables)
  - [teams_bootstrapper_download_filename](#teams_bootstrapper_download_filename)
  - [teams_bootstrapper_download_url](#teams_bootstrapper_download_url)
  - [teams_disable_autoupdate](#teams_disable_autoupdate)
  - [teams_download_dir](#teams_download_dir)
  - [teams_install_meeting_addin](#teams_install_meeting_addin)
  - [teams_installer_run_uninstall_first](#teams_installer_run_uninstall_first)
  - [teams_is_wvd_environment](#teams_is_wvd_environment)
  - [teams_remove_extract_dir](#teams_remove_extract_dir)
  - [teams_vc_redist_download_filename](#teams_vc_redist_download_filename)
  - [teams_vc_redist_download_url](#teams_vc_redist_download_url)
  - [teams_vc_redist_product_id](#teams_vc_redist_product_id)
  - [teams_web_rtc_download_filename](#teams_web_rtc_download_filename)
  - [teams_web_rtc_download_url](#teams_web_rtc_download_url)
  - [teams_x64_download_filename](#teams_x64_download_filename)
  - [teams_x64_download_url](#teams_x64_download_url)
  - [tteams_disable_autoupdate](#tteams_disable_autoupdate)
- [Discovered Tags](#discovered-tags)
- [Dependencies](#dependencies)
- [License](#license)
- [Author](#author)

---

## Requirements

- Minimum Ansible version: `2.1`


## Default Variables

### teams_bootstrapper_download_filename

Teams Bootstrapper download filename

#### Default value

```YAML
teams_bootstrapper_download_filename: teamsbootstrapper.exe
```

### teams_bootstrapper_download_url

Teams Bootstrapper download URL

#### Default value

```YAML
teams_bootstrapper_download_url: https://go.microsoft.com/fwlink/?linkid=2243204&clcid=0x409
```

### teams_disable_autoupdate

#### Default value

```YAML
teams_disable_autoupdate: true
```

### teams_download_dir

Download directory for installer files

#### Default value

```YAML
teams_download_dir: '{{ ansible_env.SystemRoot }}\temp\teams_install'
```

### teams_install_meeting_addin

Set to true to install an register Teams addin loader machine-wide

#### Default value

```YAML
teams_install_meeting_addin: true
```

### teams_installer_run_uninstall_first

Set to true to uninstall Teams first. This cause the machine-wide installer to truly update.

### teams_is_wvd_environment

Set to true if installed in Azure Virtual Desktop environment

#### Default value

```YAML
teams_is_wvd_environment: true
```

### teams_remove_extract_dir

Remove download directory at the end

#### Default value

```YAML
teams_remove_extract_dir: true
```

### teams_vc_redist_download_filename

VC Redistributable download filename

#### Default value

```YAML
teams_vc_redist_download_filename: vc_redist.x64.exe
```

### teams_vc_redist_download_url

VC Redistributable download URL

#### Default value

```YAML
teams_vc_redist_download_url: https://aka.ms/vs/17/release/vc_redist.x64.exe
```

### teams_vc_redist_product_id

VC Redistributable product ID

#### Default value

```YAML
teams_vc_redist_product_id: '{A181A302-3F6D-4BAD-97A8-A426A6499D78}'
```

### teams_web_rtc_download_filename

Web RTC download filename

#### Default value

```YAML
teams_web_rtc_download_filename: MsRdcWebRTCSvc_HostSetup_x64.msi
```

### teams_web_rtc_download_url

Web RTC download URL

#### Default value

```YAML
teams_web_rtc_download_url: https://aka.ms/msrdcwebrtcsvc/msi
```

### teams_x64_download_filename

Teams 64-bit download filename

#### Default value

```YAML
teams_x64_download_filename: MSTeams-x64.msix
```

### teams_x64_download_url

Teams 64-bit download URL

#### Default value

```YAML
teams_x64_download_url: https://go.microsoft.com/fwlink/?linkid=2196106
```

### tteams_disable_autoupdate

Disable auto-update

## Discovered Tags

**_teams-install-meeting-addin_**


## Dependencies

None.

## License

license (GPL-2.0-or-later, MIT, etc)

## Author

andif888
