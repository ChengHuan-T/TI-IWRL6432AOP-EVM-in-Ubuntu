# Required Documents & Software Tools

To ensure compatibility with this project, it is recommended to install the following specific versions of TI's official tools.

## 1. Required Tools

| NAME | Recommand Version | Download Links | Notes |
| :--- | :--- | :--- | :--- |
| **MMWAVE-L-SDK** | 05.05.04.02 | [LINK](https://www.ti.com/tool/zh-tw/MMWAVE-L-SDK) | Recommand install at `${HOME}/ti` |
| **SysConfig** | 1.27.0 | [LINK](https://www.ti.com/tool/SYSCONFIG) | Recommand install at `${HOME}/ti` |
| **TI CLANG Compiler** | 5.1.0.LTS | [LINK](https://www.ti.com/tool/download/ARM-CGT-CLANG/) | Recommand install at `${HOME}/ti` |
| **Code Composer Studio** | 20.5.0 | [LINK](https://www.ti.com/tool/CCSTUDIO) | Click **mmWave Sensors** |
| **UniFlash** | 9.4.1 | [LINK](https://www.ti.com/tool/UNIFLASH) | Using for flashing `.appimage` |
| **Radar Toolbox** | 4.00.00.05 | [LINK](https://dev.ti.com/tirex/explore/node?isTheia=false&node=A__AEIJm0rwIeU.2P1OBWwlaA__radar_toolbox__1AslXXD__LATEST) | Recommand download at `${HOME}/ti/Repo/` |

---

### MMWAVE-L-SDK
After installation, open README_FIRST_xWRL6432.html. Go to the **Getting Start**->**Download, Install and Setup SDK and Tools** page. Follow the steps to install SysConfig, CCS, and Mono Runtime.

### CCS
Unzip after downloaded, then click the **ccs_setup_xx.x.x.xxxxx.run** to install. Selete the components in the Selete Components page. (I only selete the mmWave Sensors)

After installation, run this command
```bash
sudo bash ${ccs_install_dir}/install_scripts/install_drivers.sh
```
If failed, cd to ${ccs_install_dir}/ccs/theia and run
```
sudo chown root chrome-sandbox
sudo chmod 4755 chrome-sandbox
```

