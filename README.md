Project is abandoned
==========
Q: Why?
A: It takes a lot of time to read Magento 1.X code to inject overrides. And Magento 2 is about to come out.
I achieved automatic scaling with AWS.

Magento-GAE - Magento in GAE Compatibility
===========

### Goal of this extension is to provide compatibility with Google App Engine.

Working version is available at: http://magento-gae.appspot.com/

#### Known limitations
- Amount of files is limited to 10000 (Some files were put to skiplist)
- Skin files donot exist in the scope of application
- file_exists returns false if file is in skin or gs.(gs is IO wrapper at GAE to access media storage)
- glob function returns false
- mkdir function is not covered in wrapper for gs.
- Write access to application storage is forbidden(no log file, no lock files)

#### How to deploy (TODO)
##### With Composer
##### With modman

#### Copyrights and Contribution
Feel free to contact with me and/or provide pull reqests. 

##### License

    Magento-GAE - Magento in GAE Compatibility
    Copyright (C) 2013  Kirill Morozov <kir.morozov@gmail.com>

    This program is free software: you can redistribute it and/or modify
    it under the terms of the GNU General Public License as published by
    the Free Software Foundation, either version 3 of the License, or
    (at your option) any later version.

    This program is distributed in the hope that it will be useful,
    but WITHOUT ANY WARRANTY; without even the implied warranty of
    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
    GNU General Public License for more details.

    You should have received a copy of the GNU General Public License
    along with this program.  If not, see <http://www.gnu.org/licenses/>.
