# m17n-db-sayura

## Sayura input method for Sinhalese for m17n-db

## Information about the Sayura input system

See:

https://www.sayura.net/im/

https://www.sayura.net/im/sayura.pdf

## Mapping

See the description at the top of the si-sayura.mim file and

https://www.sayura.net/im/sayura.pdf

## Dependencies

You will need to install

* ibus-m17n
* Any Unicode font supporting Sinhalese

## Installation

``` bash
$ mkdir -p ~/.m17n.d/
$ cp si-sayura.mim ~/.m17n.d/
$ ibus restart
```

Now ibus should list the newly added input method:

``` bash
$ ibus  list-engine | grep  -i sayura
  m17n:si:sayura - sayura (m17n)
```

## Adding the input method to your desktop:

### If you are  using Gnome3:

Open the regional settings in the gnome-control-center. Either from
the gnome panel by clicking on the icon showing a wrench and a
screwdriver. Then the gnome-control-center opens. Click on the flag
to go to the regional settings. You can also open the regional settings
directly by doing this on the command line:

``` bash
$ gnome-control-center region
```

In the regional settings dialog, click on the “+” button at the lower
left corner of the dialog to add an input method. In the search dialog
which opens, click on the three vertical dots at the bottom.  Enter
"sayura" into the search field. Click on “Sinhala”.  Select
“Sinhala (sayura (m17n))” and click on the “Add” button.

### If you are not using Gnome3:

Start ibus-setup and add the “sayura (m17n)” input method (Search
for “Sinhala”). Don’t use ibus-setup if you are using Gnome3, it
does not work for Gnome3!
