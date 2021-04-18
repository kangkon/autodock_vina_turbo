# Autodock Vina Turbo
Responsive version of Autodock Vina

## Requirements

- gcc/g++  9.3.0 and make - Install by `sudo apt install build-essential`, You may also want to install the manual pages about using GNU/Linux for development: `sudo apt-get install manpages-dev`
- Boost 1.76.0
- makedepend - Install by `sudo apt install xutils-dev`

## Install Instructions

Download and Extract BOOST 1.76.0 

```bash
# Create BOOST library directorie and grant required permissions
mkdir /opt/boost_c++
sudo chmod -R 777 /opt/boost_c++

# Navigate to boost extracted directory
./bootstrap.sh --prefix=/opt/boost_c++

./b2 install
```

Compile Autodock Vina

```bash
make depend
make
```