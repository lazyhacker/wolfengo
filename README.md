# WolfenGo

This is forked from http://github.com/gdm85/wolfengo.

The files were moved around to make it easier to download (single 'go get' call) and build (just use 'go build' instead of 'make'.

This is a clone of Wolfenstein3D written in Go, based on [Wolfenstein3DClone](https://github.com/BennyQBD/Wolfenstein3DClone) and licensed under [GNU/GPLv2](./LICENSE).

Pull requests are welcome.

# Build Dependencies

WolfenGo uses glfw C bindings, which in turn need some Linux userland headers to be installed. Example of dependencies installation on a Debian-based system:
```
apt-get install libxcursor-dev libxrandr-dev libxinerama-dev libxi-dev
```

# Downloading, Building, and Running

```
go get github.com/lazyhacker/wolfengo
cd $GOPATH/src/github.com/lazyhacker/wolfengo
go build
./wolfengo
```
There are some constants in `main.go` that can be toggled to enable further debugging/experimentation.

# Controls

Use `W`,`A`,`S`,`D` to move the player around and `E` to open doors; by clicking in the game window you will enable free mouse look, that can be disabled with `ESC`.

# Thanks

To gdm85 where I forked this from.

Obviously thanks to BennyQBD for the initial clone Java sources and also to https://github.com/go-gl/gl which - although not easy to master - is indeed in a good status for usage in Go OpenGL projects.
