# cilium/ebpf

## Go Embed

https://github.com/cilium/ebpf/blob/master/examples/kprobe/bpf_bpfeb.go:117

i was baffled when i learned this, but Go has the embed directive which enables you
to load binary file on disk to a bytes[] buffer for example in your go program.

kprobe example uses this ability to load into go's buffer a C-compiled ebpf code.
I guess the compile EBPF object code is then loaded into the ebpf sandbox by your
program itself.