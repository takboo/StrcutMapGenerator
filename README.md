#Struct Map Generator

这个项目的作用是读取各类Strcut源文件，然后生成对应的结构图。

样例:

源文件
```c
ClassFile {
    u4             magic;
    u2             minor_version;
    u2             major_version;
    u2             constant_pool_count;
    cp_info        constant_pool[constant_pool_count-1];
    u2             access_flags;
    u2             this_class;
    u2             super_class;
    u2             interfaces_count;
    u2             interfaces[interfaces_count];
    u2             fields_count;
    field_info     fields[fields_count];
    u2             methods_count;
    method_info    methods[methods_count];
    u2             attributes_count;
    attribute_info attributes[attributes_count];
}
```

结构图
```
               class file format
            +---------------------+
            +        magic        +
            +---------------------+
            +    minor_version    +
            +---------------------+
            +    major_version    +
            +---------------------+
            + constant_pool_count +
            +---------------------+
            +    constant_pool    +
            +---------------------+
            +     access_flag     +
            +---------------------+
            +      this_class     +
            +---------------------+
            +     super_class     +
            +---------------------+
            +  interfaces_count   +
            +---------------------+
            +      interfaces     +
            +---------------------+
            +     fields_count    +
            +---------------------+
            +       fields        +
            +---------------------+
            +    methods_count    +
            +---------------------+
            +      methods        +
            +---------------------+
            +  attributes_count   +
            +---------------------+
            +     attributes      +
            +---------------------+
```