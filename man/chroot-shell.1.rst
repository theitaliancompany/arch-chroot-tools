..
   SPDX-License-Identifier: AGPL-3.0-or-later

   ----------------------------------------------------------------------
   Copyright © 2024, 2025, 2026  Pellegrino Prevete

   All rights reserved
   ----------------------------------------------------------------------

   This program is free software: you can redistribute it and/or modify
   it under the terms of the GNU Affero General Public License as published by
   the Free Software Foundation, either version 3 of the License, or
   (at your option) any later version.

   This program is distributed in the hope that it will be useful,
   but WITHOUT ANY WARRANTY; without even the implied warranty of
   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
   GNU Affero General Public License for more details.

   You should have received a copy of the GNU Affero General Public License
   along with this program.  If not, see <https://www.gnu.org/licenses/>.


=====================================
chroot-shell
=====================================


------------------------------------------------------------------
Open and enter an host container
------------------------------------------------------------------
:Version: chroot-shell |version|
:Manual section: 1


Synopsis
========

chroot-shell *[options]* *host-directory*


Description
===========

Open an host environment, either
using 'systemd-nspawn' or 'arch-chroot'.

I'm not sure the *host-directory* argument
really works so in case run the program
from the host directory directly
just in case.


Options
=======

-t                      Chroot type, can be 'chroot'
                        or 'systemd-nspawn'


Systemd-nspawn specific options
==================================

-r y\/n                 Whether to enable support for RAID devices.

-s y\/n                 Whether to enable support for sound devices.

-g y\/n                 Whether to enable support for video devices.

-k y\/n                 Whether to enable virtualization support.


Application options
=====================

-h                      Displays help.

-v                      Enable verbose output


Bugs
====

https://github.com/themartiancompany/arch-chroot-tools/-/issues

Copyright
=========

Copyright Pellegrino Prevete. AGPL-3.0.

See also
========

.. include:: variables.rst
