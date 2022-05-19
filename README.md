# cod_1
import 'package:flutter/material.dart';
import 'package:meuapp/mycard.dart';

const Color darkBlue = Color.fromARGB(255, 18, 32, 47);

Widget myCard() {
  return Column();
}

void main() {
  runApp(MyApp());
}

class MyApp extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      theme: ThemeData.dark().copyWith(
        scaffoldBackgroundColor: darkBlue,
      ),
      debugShowCheckedModeBanner: false,
      home: Scaffold(
        body: Center(
          child: ListView(
            children: <Widget>[
              MyCard(
                name: "Alef",
                phone: "1198352-7415",
                gmail: "hahaha@gmail.com",
              ),
            ],
          ),
        ),
      ),
    );
  }
}

class MyWidget extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return Column(
        mainAxisAlignment: MainAxisAlignment.spaceEvenly, children: <Widget>[]);
  }
}

