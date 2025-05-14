# proj323-Application-dynamic-loading-enhancement
# 基于小米澎湃OS(Vela OS)应用程序动态加载增强

## 项目描述
  目前在澎湃OS（Vela with NuttX Kernel）上，已经支持ELF/NXFLAT等应用程序动态加载方案，但它们有各自的局限性，例如，ELF动态加载方案需要对代码段做重定位，导致代码必须被加载到RAM中运行，NXFLAT可以支持XIP，可以直接在Flash中运行从而节约RAM空间，但它仅能通过早期的编译器支持ARM Cortex M平台，支持的平台有限。

## 预期目标
- 基于NuttX，并使用ELF格式作为容器
- 支持XIP，可以将应用binary烧录到Flash上任意区域执行
- 适配主流平台：例如ARM和RISCV（QEMU）

## 难度：
中高

## 赛题分类
新型模块化组件（如eBPF的功能增强）

## 参考资料
- https://nuttx.apache.org
- https://refspecs.linuxbase.org/LSB_3.0.0/LSB-PDA/LSB-PDA/generic-elf.html

## 预期目标
注意：下面的内容是建议内容，不要求必须全部完成。选择本项目的同学也可与导师联系，提出自己的新想法，如导师认可，可加入预期目标
- 完善NXFLAT，适配到新版GCC并支持ARM/RISCV
- 基于ELF对加载器和编译器、编译参数等方面进行修改，例如通过-fPIC实现位置无关

## 所属赛道
2025全国大学生操作系统比赛的“OS功能挑战”赛道

## 指导专家介绍及联系方式
- 黄齐，Bytecode Alliance RC / WAMR TSC Member , huangqi3@xiaomi.com
- 小米公司Vela研发团队（含NuttX社区主要代码提交人）

## 对参赛队提供的支持
- NuttX的内核实现和动态加载器
- 针对NuttX实时操作系统业界最专业和权威的技术支持
