

- Downloads local repos  cuda-repo-ubuntu2204-11-8-local_11.8.0-520.61.05-1_amd64.deb  nv-tensorrt-local-repo-ubuntu2204-8.6.1-cuda-11.8_1.0-1_amd64.deb

    ```console
    $ sudo dpkg -i nv-tensorrt-local-repo-ubuntu2204-8.6.1-cuda-11.8_1.0-1_amd64.deb
    $ sudo cp /var/nv-tensorrt-local-repo-ubuntu2204-8.6.1-cuda-11.8/*-keyring.gpg /usr/share/keyrings/
    $ sudo apt update
    ```
    
 - Go to the folder /var/nv-tensorrt-local-repo-ubuntu2204-8.6.1-cuda-11.8 and add each package manually
     ```console
	$ sudo dpkg -i libnvinfer8_8.6.1.6-1+cuda11.8_amd64.deb
	$ sudo dpkg -i libnvinfer-headers-dev_8.6.1.6-1+cuda11.8_amd64.deb
	$ sudo dpkg -i libnvinfer-dev_8.6.1.6-1+cuda11.8_amd64.deb
	$ sudo dpkg -i libnvinfer-plugin8_8.6.1.6-1+cuda11.8_amd64.deb
	$ sudo dpkg -i libnvinfer-headers-plugin-dev_8.6.1.6-1+cuda11.8_amd64.deb
	$ sudo dpkg -i libnvinfer-plugin-dev_8.6.1.6-1+cuda11.8_amd64.deb
	$ sudo dpkg -i libnvonnxparsers8_8.6.1.6-1+cuda11.8_amd64.deb
	$ sudo dpkg -i libnvonnxparsers-dev_8.6.1.6-1+cuda11.8_amd64.deb
	$ sudo dpkg -i onnx-graphsurgeon_8.6.1.6-1+cuda11.8_amd64.deb
	$ sudo dpkg -i libnvparsers8_8.6.1.6-1+cuda11.8_amd64.deb
	$ sudo dpkg -i libnvparsers-dev_8.6.1.6-1+cuda11.8_amd64.deb
	$ sudo dpkg -i libnvinfer-lean8_8.6.1.6-1+cuda11.8_amd64.deb
	$ sudo dpkg -i libnvinfer-vc-plugin8_8.6.1.6-1+cuda11.8_amd64.deb
	$ sudo dpkg -i libnvinfer-dispatch8_8.6.1.6-1+cuda11.8_amd64.deb
	$ sudo dpkg -i libnvinfer-bin_8.6.1.6-1+cuda11.8_amd64.deb
	$ sudo dpkg -i libnvinfer-lean-dev_8.6.1.6-1+cuda11.8_amd64.deb
	$ sudo dpkg -i libnvinfer-vc-plugin-dev_8.6.1.6-1+cuda11.8_amd64.deb
	$ sudo dpkg -i libnvinfer-dispatch-dev_8.6.1.6-1+cuda11.8_amd64.deb
	$ sudo dpkg -i libnvinfer-samples_8.6.1.6-1+cuda11.8_all.deb
	$ sudo dpkg -i tensorrt_8.6.1.6-1+cuda11.8_amd64.deb
    ```
 
 - If you need additional cuda dependencies, install them from the local repository.
     ```console
    $ sudo dpkg -i cuda-repo-ubuntu2204-11-8-local_11.8.0-520.61.05-1_amd64.deb
    ```
    
 - Checking the installed version
      ```console
     $ dpkg-query -W tensorrt 
    ```
