# Software Installation

Workshop attendees may wish to follow along by running the FloPy/MODFLOW 6 examples.  This will require that software be installed prior to the workshop.  Required software includes:

1.  Python (preferably 3.10 or newer).  [miniforge](https://github.com/conda-forge/miniforge/releases) is a popular Python distribution that runs on Windows, Mac, and Linux. Note that you may have to expand the list to find you operating system by following a link called that says `Show all 74 assets`

2.  Use conda to install a customized environment for FloPy and MODFLOW. 
Run the following command from a terminal in the folder `.\installation`.

```
$ mamba env create -f flopy_environment.yml
```

Whenever you want to use this FloPy environment, you will need to activate it with the following command.

```
conda activate flopy
```

3.  Install MODFLOW executables and related programs.  After FloPy has been installed, MODFLOW executables can be downloaded to your computer using the [get-modflow](https://github.com/modflowpy/flopy/blob/develop/docs/get_modflow.md) utility, which is installed with FloPy. The following command is one way to use `get-modflow`, which will download the executables and make them available for use with FloPy scripts.  Make sure that the flopy environment is active before you run `get-modflow`.

```
$ get-modflow :flopy 
```

4. You are ready to go!