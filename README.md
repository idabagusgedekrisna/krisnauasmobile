{
    // Use IntelliSense to learn about possible attributes.
    // Hover to view descriptions of existing attributes.
    // For more information, visit: https://go.microsoft.com/fwlink/?linkid=830387
    "version": "0.2.0",
    "configurations": [
        {
            "name": "Flutter",
            "request": "launch",
            "type": "dart"
        }
    ]
}
name: uas_mobile
description: A new Flutter project.

# The following defines the version and build number for your application.
# A version number is three numbers separated by dots, like 1.2.43
# followed by an optional build number separated by a +.
# Both the version and the builder number may be overridden in flutter
# build by specifying --build-name and --build-number, respectively.
# In Android, build-name is used as versionName while build-number used as versionCode.
# Read more about Android versioning at https://developer.android.com/studio/publish/versioning
# In iOS, build-name is used as CFBundleShortVersionString while build-number used as CFBundleVersion.
# Read more about iOS versioning at
# https://developer.apple.com/library/archive/documentation/General/Reference/InfoPlistKeyReference/Articles/CoreFoundationKeys.html
version: 1.0.0+1

environment:
  sdk: ">=2.1.0 <3.0.0"

dependencies:
  flutter:
    sdk: flutter

  # The following adds the Cupertino Icons font to your application.
  # Use with the CupertinoIcons class for iOS style icons.
  cupertino_icons: ^0.1.2
  webview_flutter: 0.3.20+2
  sqflite: ^1.1.0
  path_provider: ^0.5.0+1

dev_dependencies:
  flutter_test:
    sdk: flutter


# For information on the generic Dart part of this file, see the
# following page: https://dart.dev/tools/pub/pubspec

# The following section is specific to Flutter.
flutter:

  # The following line ensures that the Material Icons font is
  # included with your application, so that you can use the icons in
  # the material Icons class.
  uses-material-design: true

  # To add assets to your application, add an assets section, like this:
  assets:
    - images/arikusuma.jpg

  # An image asset can refer to one or more resolution-specific "variants", see
  # https://flutter.dev/assets-and-images/#resolution-aware.

  # For details regarding adding assets from package dependencies, see
  # https://flutter.dev/assets-and-images/#from-packages

  # To add custom fonts to your application, add a fonts section here,
  # in this "flutter" section. Each entry in this list should have a
  # "family" key with the font family name, and a "fonts" key with a
  # list giving the asset and other descriptors for the font. For
  # example:
  # fonts:
  #   - family: Schyler
  #     fonts:
  #       - asset: fonts/Schyler-Regular.ttf
  #       - asset: fonts/Schyler-Italic.ttf
  #         style: italic
  #   - family: Trajan Pro
  #     fonts:
  #       - asset: fonts/TrajanPro.ttf
  #       - asset: fonts/TrajanPro_Bold.ttf
  #         weight: 700
  #
  # For details regarding fonts from package dependencies,
  # see https://flutter.dev/custom-fonts/#from-packages
  # uas_mobile
  <?xml version="1.0" encoding="UTF-8"?>
<module type="JAVA_MODULE" version="4">
  <component name="NewModuleRootManager" inherit-compiler-output="true">
    <exclude-output />
    <content url="file://$MODULE_DIR$">
      <sourceFolder url="file://$MODULE_DIR$/lib" isTestSource="false" />
      <sourceFolder url="file://$MODULE_DIR$/test" isTestSource="true" />
      <excludeFolder url="file://$MODULE_DIR$/.dart_tool" />
      <excludeFolder url="file://$MODULE_DIR$/.idea" />
      <excludeFolder url="file://$MODULE_DIR$/.pub" />
      <excludeFolder url="file://$MODULE_DIR$/build" />
    </content>
    <orderEntry type="sourceFolder" forTests="false" />
    <orderEntry type="library" name="Dart SDK" level="project" />
    <orderEntry type="library" name="Flutter Plugins" level="project" />
    <orderEntry type="library" name="Dart Packages" level="project" />
  </component>
</module>

A new Flutter project.

## Getting Started

This project is a starting point for a Flutter application.

A few resources to get you started if this is your first Flutter project:

- [Lab: Write your first Flutter app](https://flutter.dev/docs/get-started/codelab)
- [Cookbook: Useful Flutter samples](https://flutter.dev/docs/cookbook)

For help getting started with Flutter, view our
[online documentation](https://flutter.dev/docs), which offers tutorials,
samples, guidance on mobile development, and a full API reference.
<nav class="pagination-single section-inner" aria-label="Post" role="navigation">

		<hr class="styled-separator is-style-wide" aria-hidden="true">

		<div class="pagination-single-inner">

			
				<a class="previous-post" href="http://krisnamanuaba.com/2020/04/19/calculating-bmi/">
					<span class="arrow" aria-hidden="true">←</span>
					<span class="title"><span class="title-inner">CALCULATING BMI</span></span>
				</a>

				
				<a class="next-post" href="http://krisnamanuaba.com/2020/04/19/berkenalan-dengan-html/">
					<span class="arrow" aria-hidden="true">→</span>
						<span class="title"><span class="title-inner">BERKENALAN DENGAN HTML</span></span>
				</a>
				
		</div><!-- .pagination-single-inner -->

		<hr class="styled-separator is-style-wide" aria-hidden="true">

	</nav>
    import 'package:flutter/material.dart';
import 'Wview.dart';

class MyProfil extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return
      Scaffold(
          backgroundColor: Colors.lightBlue[100],
          appBar: AppBar(
            title: Text("Profil Pembuat Aplikasi"),
            centerTitle: true,
            bottom: PreferredSize(
                child: Container(
                  color:Colors.black,
                  height: 4.0,
                ),
                preferredSize: null
            ),
          ),
          body: Konten()
      );
  }
}

class Konten extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return
      new Scaffold(
        body: ListView(
          children: <Widget>[
            Container(
              color: Colors.white,
              child: Stack(
                children: <Widget>[
                  Padding(
                    padding: EdgeInsets.only(top: 5),
                    child: Align(
                      alignment: Alignment.topCenter,
                      child: Container(
                        height: 200,
                        width: 200,
                        decoration: BoxDecoration(
                            borderRadius: BorderRadius.circular(100),
                            image: DecorationImage(image: AssetImage('images/arikusuma.jpg'),
                                fit: BoxFit.cover
                            )
                        ),
                      ),
                    ),
                  ),
                ],
              ),
            ),

            Container(
              color: Colors.white,
              child: Column(

                children: <Widget>[
                  SizedBox(height: 20),
                  Text('Komang Ari Kusuma',
                    style: TextStyle(
                      fontWeight: FontWeight.bold,
                      fontSize: 22,
                      color: Colors.black,
                    ),
                  ),
                  SizedBox(height: 5,child: Container(
                    color: Colors.white,
                  ),),
                  Row(
                    mainAxisAlignment: MainAxisAlignment.center,
                    children: <Widget>[
                      Text('Pendidikan Teknik Informatika',
                        style: TextStyle(
                            fontWeight: FontWeight.bold,
                            fontSize: 20,
                            color: Colors.black
                        ),
                      )

                    ],
                  ),
                ],
              ),
            ),
            Container(
              padding: EdgeInsets.only(top: 30, right: 50, left: 50),
              child: Column(
                children: <Widget>[
                  Padding(
                    padding: const EdgeInsets.all(0),
                    child: Row(
                      mainAxisAlignment: MainAxisAlignment.spaceBetween,
                      children: <Widget>[
                        Container(
                          height: 100,
                          width: 100,
                          decoration: BoxDecoration(
                            border: Border.all(color: Colors.black),
                            //color: Colors.green,
                            borderRadius: BorderRadius.only(topRight: Radius.circular(20), topLeft: Radius.circular(20)),

                          ),

                          child: Padding(
                            padding: const EdgeInsets.all(12.0),
                            child: Column(
                              children: <Widget>[
                                IconButton(
                            icon: Icon(Icons.my_location, color: Colors.black, size: 38),
                            onPressed: () {
                              Navigator.push(
                                context,
                                MaterialPageRoute(builder: (context) => Wview()),
                              );
                            },
                          ),
                          Container(
                            child: Text('Bali', style: 
                            TextStyle(color: Colors.black54,
                                    fontWeight: FontWeight.bold),
                            ),
                            padding: EdgeInsets.all(5),
                          )
                              ],
                            ),
                          ),
                        ),

                        Container(
                          height: 100,
                          width: 100,
                          decoration: BoxDecoration(
                            border: Border.all(color: Colors.black),
                            //color: Colors.green,
                            borderRadius: BorderRadius.only(topRight: Radius.circular(20), topLeft: Radius.circular(20)),
                          ),

                          child: Padding(
                            padding: const EdgeInsets.all(12.0),
                            child: Column(
                              children: <Widget>[
                                Icon(Icons.home, color: Colors.black, size: 58,),
                                Text('Liligundi', style: TextStyle
                                  (color: Colors.black54,
                                    fontWeight: FontWeight.bold
                                ),
                                ),
                              ],
                            ),
                          ),
                        ),

                      ],
                    ),
                  ),
                  Padding(
                    padding: const EdgeInsets.only(top: 40),
                    child: Row(
                      mainAxisAlignment: MainAxisAlignment.spaceBetween,
                      children: <Widget>[
                        Container(

                          height: 100,
                          width: 100,
                          decoration: BoxDecoration(
                            border: Border.all(color: Colors.black),
                            //color: Colors.green ,
                            borderRadius: BorderRadius.only(topRight: Radius.circular(20), topLeft: Radius.circular(20)),


                          ),

                          child: Padding(
                            padding: const EdgeInsets.all(12.0),
                            child: Column(
                              children: <Widget>[
                                Icon(Icons.music_note,color: Colors.black, size: 58,),
                                Text('POP', style: TextStyle
                                  (color: Colors.black54,
                                    fontWeight: FontWeight.bold
                                ),
                                ),
                              ],
                            ),
                          ),
                        ),
                        Container(

                          height: 100,
                          width: 100,
                          decoration: BoxDecoration(
                            border: Border.all(color: Colors.black),
                            borderRadius: BorderRadius.only(topRight: Radius.circular(20), topLeft: Radius.circular(20)),
                          ),

                          child: Padding(
                            padding: const EdgeInsets.all(12.0),
                            child: Column(
                              children: <Widget>[
                                Icon(Icons.school, color: Colors.black, size: 58,),
                                Text('Undiksha',style: TextStyle
                                  (color: Colors.black54,
                                    fontWeight: FontWeight.bold
                                ),
                                ),
                              ],
                            ),
                          ),
                        )
                      ],
                    ),
                  )
                ],
              ),
            )
          ],
        ),
      );
  }
}



import 'package:flutter/material.dart';
import 'package:flutter/rendering.dart';
import 'package:uas_mobile/ui/note.dart';

import 'Output.dart';
import 'about_me.dart.';

class InputData extends StatefulWidget {
  @override
  _InputDataState createState() => _InputDataState();
}

class _InputDataState extends State<InputData> {
  TextEditingController nama = TextEditingController();
  TextEditingController alamat = TextEditingController();
  int pokok = 0;
  int bunga = 0;
  int tahun = 0;

  @override
  Widget build(BuildContext context) {
    return Scaffold(
      backgroundColor: Colors.blueGrey[100],
      appBar: AppBar(
        leading: IconButton(
          icon: Icon(Icons.face, color: Colors.white, size: 30),
            onPressed: () {
              Navigator.push(
                context,
                MaterialPageRoute(builder: (context) => MyProfil()),
              );
            },
        ),
        title: Text('      '),
        actions: <Widget>[
          IconButton(
            icon: Icon(Icons.note_add, color: Colors.white, size: 30),
            onPressed: () {
              Navigator.push(
                context,
                MaterialPageRoute(builder: (context) => Note()),
              );
            },
          ),
        ],
        bottom: PreferredSize(
            child: Container(
              color: Colors.black,
              height: 4.0,
            ),
            preferredSize: null),
      ),
      body: SingleChildScrollView(
        child: Column(
          crossAxisAlignment: CrossAxisAlignment.stretch,
          mainAxisAlignment: MainAxisAlignment.start,
          children: <Widget>[
            Container(
              padding: EdgeInsets.all(12),
              color: Colors.blue,
              child: Column(
                children: <Widget>[
                  Text(
                    'APLIKASI ',
                    style: TextStyle(
                        color: Colors.white,
                        fontSize: 23.0,
                        fontWeight: FontWeight.w500),
                  ),
                  Text(
                    'Menghitung Bunga Rupiah',
                    style: TextStyle(
                        color: Colors.white,
                        fontSize: 23.0,
                        fontWeight: FontWeight.w500),
                  ),
                ],
              ),
            ),
            Container(
                margin: EdgeInsets.only(top: 5),
                padding: EdgeInsets.all(5),
                child: Column(
                  children: <Widget>[
                    SizedBox(
                    height: 22,
                  ),
                    TextField(
                      controller: nama,
                      decoration: InputDecoration(
                        hintText: "Masukkan Nama Peminjam",
                        labelText: "Nama Lengkap",
                        border: OutlineInputBorder(
                          borderRadius: BorderRadius.circular(10.0),
                        ),
                      ),
                    ),
                    SizedBox(
                    height: 22,
                  ),
                    TextField(
                      controller: alamat,
                      decoration: InputDecoration(
                        hintText: "Masukkan Alamat Peminjam",
                        labelText: "Alamat",
                        border: OutlineInputBorder(
                          borderRadius: BorderRadius.circular(10.0),
                        ),
                      ),
                    ),
                    SizedBox(
                    height: 22,
                  ),
                    TextField(
                      onChanged: (txt) {
                        setState(() {
                          pokok = int.parse(txt);
                        });
                      },
                      style: TextStyle(
                        fontSize: 15,
                      ),
                      decoration: InputDecoration(
                          labelText: "Jumlah Pokok Rupiah",
                          suffix: Text('Rupiah'),
                          border: OutlineInputBorder(
                              borderRadius: BorderRadius.circular(10.0)),
                          hintText: 'Jumlah uang'),
                    ),
                    
                    SizedBox(
                    height: 22,
                  ),
                    TextField(
                      onChanged: (txt) {
                        setState(() {
                          bunga = int.parse(txt);
                        });
                      },
                      style: TextStyle(
                        fontSize: 15,
                      ),
                      decoration: InputDecoration(
                          labelText: "Besar Bunga",
                          suffix: Text('%'),
                          border: OutlineInputBorder(
                              borderRadius: BorderRadius.circular(10.0)),
                          hintText: 'percent'),
                    ),
                    
                    SizedBox(
                    height: 22,
                  ),
                    TextField(
                      onChanged: (txt) {
                        setState(() {
                          tahun = int.parse(txt);
                        });
                      },
                      style: TextStyle(
                        fontSize: 15,
                      ),
                      decoration: InputDecoration(
                          labelText: "Durasi",
                          suffix: Text('Tahun'),
                          border: OutlineInputBorder(
                              borderRadius: BorderRadius.circular(10.0)),
                          hintText: 'Tahun'),
                    ),
                  ],
                )),
            Container(
              margin: EdgeInsets.only(left: 70, right: 70, bottom: 20),
              child: RaisedButton(
                onPressed: () {
                  _sendDataTobmiResult(context);
                },
                padding: EdgeInsets.only(top: 5, bottom: 5),
                color: Colors.blue,
                child: Text(
                  'Hitung',
                  style: TextStyle(fontSize: 20, fontWeight: FontWeight.w500),
                ),
                shape: RoundedRectangleBorder(
                    borderRadius: BorderRadius.circular(40)),
              ),
            ),
          ],
        ),
      ),
      bottomNavigationBar: BottomAppBar(
      ),
    );
  }

  void _sendDataTobmiResult(BuildContext context) {
    String textToSend = nama.text;
    String text = alamat.text;
    Navigator.push(
        context,
        MaterialPageRoute(
            builder: (context) => OutputAPK(
                  nama: textToSend,
                  alamat: text,
                  pokokpinjaman: pokok,
                  bungapinjaman: bunga,
                  durasi: tahun,
                )
              )
            );
  }
}
import 'package:flutter/material.dart';
import 'input.dart';

void main() => runApp(
    MaterialApp(
      debugShowCheckedModeBanner: false,
      theme: ThemeData(
        primarySwatch: Colors.grey
      ),
      home:  InputData(),
    )
);
import 'package:flutter/material.dart';

class OutputAPK extends StatelessWidget {
  OutputAPK(
    {
      @required this.nama,
      @required this.alamat,
      @required this.pokokpinjaman,
      @required this.bungapinjaman,
      @required this.durasi
    }
  );

  final int pokokpinjaman;
  final int bungapinjaman;
  final int durasi;
  final String nama;
  final String alamat;

  @override
  Widget build(BuildContext context) {
    double jumlahPokok = pokokpinjaman + (pokokpinjaman * bungapinjaman * durasi) / 100;
    double jumlahbunga = (jumlahPokok - pokokpinjaman);
    return Scaffold(
      backgroundColor: Colors.blueGrey[100],
      appBar: AppBar(
        centerTitle: true,
        title: Text('Hasil'),
        bottom: PreferredSize(
            child: Container(
              color: Colors.blue[500],
              height: 4.0,
            ),
            preferredSize: null),
      ),

      body: Center(
        child: Column(
          children: <Widget>[
            
            Container(
              padding: EdgeInsets.all(4),
              color: Colors.black,
            ),

            Container(
              margin: EdgeInsets.only(top: 15),
              padding: EdgeInsets.only(left: 10, right: 10, bottom: 5),
              decoration: BoxDecoration(
                  color: Colors.blue[100],
                  borderRadius: BorderRadius.circular(20),
                  border: Border.all(
                    color: Colors.blue,
                    width: 5,
                  )
                ),

                child: Column(
                  children: <Widget>[
                    Container(
                      child: Text(
                        'Hasil Akumulasi Pinjaman',
                        style: TextStyle(
                            color: Colors.black,
                            fontSize: 17.0,
                            fontWeight: FontWeight.w600),
                      ),
                      padding: EdgeInsets.only(left: 70, right: 50, top:5, bottom:5 ),
                      decoration: BoxDecoration(
                        color: Colors.blue,
                        borderRadius: BorderRadius.circular(30),
                        border: Border.all(
                          color: Colors.black,
                          width: 2,
                        )
                      ),
                    ),
                    
                    Text(
                      "Nama Peminjam",
                      style: TextStyle(
                        fontSize: 17,
                        fontWeight: FontWeight.w800,
                      ),
                    ),
                    
                    Text(
                      "$nama",
                      style: TextStyle(
                          fontSize: 17,
                          fontWeight: FontWeight.w800,
                          color: Colors.red),
                    ),

                    Text(
                      "Alamat Peminjam",
                      style: TextStyle(
                        fontSize: 17,
                        fontWeight: FontWeight.w800,
                      ),
                    ),

                    Text(
                      "$alamat",
                      style: TextStyle(
                          fontSize: 17,
                          fontWeight: FontWeight.w800,
                          color: Colors.red),
                    ),

                    Text(
                      "Jumlah Pokok Rupiah",
                      style: TextStyle(
                        fontSize: 17,
                        fontWeight: FontWeight.w800,
                      ),
                    ),

                    Text(
                      "$pokokpinjaman",
                      style: TextStyle(
                          fontSize: 17,
                          fontWeight: FontWeight.w800,
                          color: Colors.red),
                    ),

                    Text(
                      "Besar Bunga",
                      style: TextStyle(
                          fontSize: 17, fontWeight: FontWeight.w800),
                    ),

                    Text(
                      "$bungapinjaman%",
                      textAlign: TextAlign.right,
                      style: TextStyle(
                          fontSize: 17,
                          fontWeight: FontWeight.w800,
                          color: Colors.red),
                    ),

                    Text(
                      "durasi",
                      style: TextStyle(
                          fontSize: 17, fontWeight: FontWeight.w800),
                    ),

                    Text(
                      "$durasi Tahun",
                      textAlign: TextAlign.start,
                      style: TextStyle(
                          fontSize: 17,
                          fontWeight: FontWeight.w800,
                          color: Colors.red),
                    ),

                     Text(
                      "Total Bunga ",
                      style: TextStyle(
                          fontSize: 17, fontWeight: FontWeight.w800),
                    ),

                    Text(
                      "$jumlahbunga",
                      textAlign: TextAlign.right,
                      style: TextStyle(
                          fontSize: 17,
                          fontWeight: FontWeight.w800,
                          color: Colors.red),
                    ),


                    Text(
                      "Total Pokok Rupiah Beserta Bunga",
                      style: TextStyle(
                          fontSize: 17, fontWeight: FontWeight.w800),
                    ),

                    Text(
                      "$jumlahPokok",
                      textAlign: TextAlign.start,
                      style: TextStyle(
                          fontSize: 17,
                          fontWeight: FontWeight.w800,
                          color: Colors.red),
                    )
                  ],
                )
              ),
              
              Container(
              margin: EdgeInsets.only(left: 60, right: 60,top:20, bottom: 20),
              child: RaisedButton(
                 onPressed: () {
                    Navigator.pop(context);
                  },
                padding: EdgeInsets.only(top: 5, bottom: 5),
                color: Colors.blue,
                child: Text(
                  'Kembali',
                  style: TextStyle(fontSize: 20, fontWeight: FontWeight.w500),
                ),
                shape: RoundedRectangleBorder(
                    borderRadius: BorderRadius.circular(40)),
              ),
            ),
          ],
        ),
      ),
    );
  }
}
import 'package:flutter/material.dart';
import 'package:uas_mobile/models/anggota.dart';

class EntryForm extends StatefulWidget {
  final Anggota anggota;
  EntryForm(this.anggota);
  @override
  EntryFormState createState() => EntryFormState(this.anggota);
}

class EntryFormState extends State<EntryForm> {
  Anggota anggota;
  EntryFormState(this.anggota);
  TextEditingController namaController = TextEditingController();
  TextEditingController alamatController = TextEditingController();
  TextEditingController nomorController = TextEditingController();

  @override
  Widget build(BuildContext context) {
    if (anggota != null) {
      namaController.text = anggota.nama;
      alamatController.text = anggota.alamat;
      nomorController.text = anggota.nomor;
    }

    return Scaffold(
       backgroundColor: Colors.white,
        appBar: AppBar(
          title: anggota == null ? Text('Tambah') : Text('Edit'),
          centerTitle: true,
          bottom: PreferredSize(
          child: Container(
            color:Colors.blue[500],
            height: 4.0,
          ),
          preferredSize: null
        ),
        ),
        body: Padding(
          padding: EdgeInsets.only(top: 15.0, left:10.0, right:10.0),
          child: ListView(
            children: <Widget> [
              Padding (
                padding: EdgeInsets.only(top:20.0, bottom:20.0),
                child: TextField(
                  controller: namaController,
                  keyboardType: TextInputType.text,
                  decoration: InputDecoration(
                    labelText: 'nama',
                    border: OutlineInputBorder(
                      borderRadius: BorderRadius.circular(5.0),
                    ),
                  ),
                  onChanged: (value) {
                    //
                  },
                ),
              ),

              Padding (
                padding: EdgeInsets.only(top:20.0, bottom:20.0),
                child: TextField(
                  controller: alamatController,
                  keyboardType: TextInputType.text,
                  decoration: InputDecoration(
                    labelText: 'Alamat',
                    border: OutlineInputBorder(
                      borderRadius: BorderRadius.circular(5.0),
                    ),
                  ),
                  onChanged: (value) {
                    //
                  },
                ),
              ),

              Padding (
                padding: EdgeInsets.only(top:20.0, bottom:20.0),
                child: TextField(
                  controller: nomorController,
                  keyboardType: TextInputType.text,
                  decoration: InputDecoration(
                    labelText: 'No Hp',
                    border: OutlineInputBorder(
                      borderRadius: BorderRadius.circular(5.0),
                    ),
                  ),
                  onChanged: (value) {
                    //
                  },
                ),
              ),

              Padding (
                padding: EdgeInsets.only(top:10.0, bottom:10.0),
                child: Row(
                  children: <Widget> [
                    Expanded(
                      child: RaisedButton(
                        color: Colors.blue,
                        textColor: Colors.white,
                        child: Text(
                          'Simpan',
                          textScaleFactor: 1.5,
                        ),
                        onPressed: () {
                          if (anggota == null) {
                            anggota = Anggota(namaController.text, alamatController.text, nomorController.text);
                          } else {
                            anggota.nama = namaController.text;
                            anggota.alamat = alamatController.text;
                            anggota.nomor= nomorController.text;
                          }
                          Navigator.pop(context, anggota);
                        },
                      ),
                    ),
                    Container(width: 5.0,),
                    Expanded(
                      child: RaisedButton(
                        color: Colors.red,
                        textColor: Colors.white,
                        child: Text(
                          'Batal',
                          textScaleFactor: 1.5,
                        ),
                        onPressed: () {
                          Navigator.pop(context);
                        },
                      ),
                    ),
                  ],
                ),
              ),
            ],
          ),
        )
    );
  }
}
import 'package:flutter/material.dart';
import 'package:uas_mobile/ui/entryForm.dart';
import 'package:uas_mobile/models/anggota.dart';
import 'package:uas_mobile/helpers/hdatabases.dart';
import 'package:sqflite/sqflite.dart';
import 'dart:async';

class Note extends StatefulWidget {
  @override
  NoteState createState() => NoteState();
}

class NoteState extends State<Note> {
  DbHelper dbHelper = DbHelper();
  int count = 0;
  List<Anggota> anggotaList;

  @override
  Widget build(BuildContext context) {
    if (anggotaList == null) {
      anggotaList = List<Anggota>();
    }

    return Scaffold(
      backgroundColor: Colors.white,
      appBar: AppBar(
        title: Text('Anggota'),
        centerTitle: true,
        bottom: PreferredSize(
          child: Container(
            color:Colors.blue[500],
            height: 4.0,
          ),
          preferredSize: null
        ),
      ),
      body: createListView(),
      floatingActionButton: FloatingActionButton(
        child: Icon(Icons.add),
        tooltip: 'Tambah Data',
        onPressed: () async {
          var anggota = await navigateToEntryForm(context, null);
          if (anggota != null) addAnggota(anggota);
        },
      ),
    );
  }

  Future<Anggota> navigateToEntryForm(BuildContext context, Anggota anggota) async {
    var result = await Navigator.push(
        context,
        MaterialPageRoute(
            builder: (BuildContext context) {
              return EntryForm(anggota);
            }
        )
    );
    return result;
  }

  ListView createListView() {
    TextStyle textStyle = Theme.of(context).textTheme.subhead;
    return ListView.builder(
      itemCount: count,
      itemBuilder: (BuildContext context, int index) {
        return Card(
          color: Colors.blue[200],
          elevation: 2.0,
          child: ListTile(
            leading: CircleAvatar(
              backgroundColor: Colors.blue,
              child: Icon(Icons.note, color: Colors.green[800]),
            ),
            title: Text(' '+this.anggotaList[index].nama, style: textStyle,),
            subtitle: Text(' '+this.anggotaList[index].alamat + ' |  ' + this.anggotaList[index].nomor),
            trailing: GestureDetector(
              child: Icon(Icons.delete, color: Colors.red,),
              onTap: () {
                deleteAnggota(anggotaList[index]);
              },
            ),
            onTap: () async {
              var anggota = await navigateToEntryForm(context, this.anggotaList[index]);
              if (anggota != null) editAnggota(anggota);
            },
          ),
        );
      },
    );
  }
  
  void addAnggota(Anggota object) async {
    int result = await dbHelper.insert(object);
    if (result > 0) {
      updateListView();
    }
  }
  
  void editAnggota(Anggota object) async {
    int result = await dbHelper.update(object);
    if (result > 0) {
      updateListView();
    }
  }
  
  void deleteAnggota(Anggota object) async {
    int result = await dbHelper.delete(object.id);
    if (result > 0) {
      updateListView();
    }
  }
  
  void updateListView() {
    final Future<Database> dbFuture = dbHelper.initDb();
    dbFuture.then((database) {
      Future<List<Anggota>> anggotaListFuture = dbHelper.getAnggotaList();
      anggotaListFuture.then((anggotaList) {
        setState(() {
          this.anggotaList = anggotaList;
          this.count = anggotaList.length;
        });
      });
    });
  }
}
    class Anggota {
  int _id;
  String _nama;
  String _alamat;
  String _nomor;
  
  Anggota(this._nama, this._alamat, this._nomor);

  Anggota.fromMap(Map<String, dynamic> map) {
    this._id = map['id'];
    this._nama = map['nama'];
    this._alamat = map['alamat'];
    this._nomor = map['nomor'];
  }

  // getter
  int get id => _id;
  String get nama => _nama;
  String get alamat => _alamat;
  String get nomor => _nomor;

  // setter
  set nama(String value) {
    _nama = value;
  }

  set alamat(String value) {
    _alamat = value;
  }

  set nomor(String value) {
    _nomor = value;
  }

  Map<String, dynamic> toMap() {
    Map<String, dynamic> map = Map<String, dynamic>();
    map['id'] = this._id;
    map['nama'] = nama;
    map['alamat'] = alamat;
    map['nomor'] = nomor;
    return map;
  }
}
import 'package:sqflite/sqflite.dart';
import 'dart:async';
import 'dart:io';
import 'package:path_provider/path_provider.dart';
import 'package:uas_mobile/models/anggota.dart';

class DbHelper {
  static DbHelper _dbHelper;
  static Database _database;
  DbHelper._createObject();
  factory DbHelper() {
    if (_dbHelper == null) {
      _dbHelper = DbHelper._createObject();
    }
    return _dbHelper;
  }

  Future<Database> initDb() async {
    Directory directory = await getApplicationDocumentsDirectory();
    String path = directory.path + 'angota.db';
    var todoDatabase = openDatabase(path, version: 1, onCreate: _createDb);
    return todoDatabase;
  }

  void _createDb(Database db, int version) async {
    await db.execute('''
      CREATE TABLE anggota (
        id INTEGER PRIMARY KEY AUTOINCREMENT,
        nama TEXT,
        alamat TEXT,
        nomor TEXT
      )
    ''');
  }

  Future<Database> get database async {
    if (_database == null) {
      _database = await initDb();
    }
    return _database;
  }

  Future<List<Map<String, dynamic>>> select() async {
    Database db = await this.database;
    var mapList = await db.query('anggota', orderBy: 'nama');
    return mapList;
  }

  Future<int> insert(Anggota object) async {
    Database db = await this.database;
    int count = await db.insert('anggota', object.toMap());
    return count;
  }

  Future<int> update(Anggota object) async {
    Database db = await this.database;
    int count = await db.update('anggota', object.toMap(),
        where: 'id=?',
        whereArgs: [object.id]);
    return count;
  }

  Future<int> delete(int id) async {
    Database db = await this.database;
    int count = await db.delete('anggota',
        where: 'id=?',
        whereArgs: [id]);
    return count;
  }

  Future<List<Anggota>> getAnggotaList() async {
    var anggotaMapList = await select();
    int count = anggotaMapList.length;
    List<Anggota> anggotaList = List<Anggota>();
    for (int i=0; i<count; i++) {
      anggotaList.add(Anggota.fromMap(anggotaMapList[i]));
    }
    return anggotaList;
  }
}
                           
