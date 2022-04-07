import 'package:flutter/material.dart';
import 'package:flutter_app_todoa/screens/home_page.dart';
import 'package:provider/provider.dart';

import 'data/data_collection.dart';

void main() {
runApp(MyApp());
}

class MyApp extends StatelessWidget {
@override
Widget build(BuildContext context) {
return ChangeNotifierProvider(
create: (_) => DataCollection(),
child: MaterialApp(
debugShowCheckedModeBanner: false,
title: 'App',
theme: ThemeData(
backgroundColor: Colors.grey,
primarySwatch: Colors.blue,
),
home: HomePage(),
),
);
}
}
