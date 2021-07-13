[TOC]

# js起源

js是1995年由网景公司开发的。ECMAScript是js的标准，js是ECMAScript的实现。

浏览器中的js包含js、DOM、BOM。nodejs中仅仅是js，不包含DOM、BOM。

## js的基本包装类型



String、Boolean、Number这三种。

当直接使用字面量调用方法的时候，js引擎就会在后台的当前行创建一个基本包装类型对象，然后调用对象的方法，并且自动销毁这个基本包装类型对象。比如调用''.toString();那么js引擎就会自动创建一个String()基本包装类型,然后调用类型的toString()原型方法，最后销毁这个基本包装类型。这个过程是在一行内就完成的，所以在下一行中我们无法使用这个基本包装类型。