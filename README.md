import 'package:flutter/material.dart';

void main() {
  runApp(const NiliApp());
}

class NiliApp extends StatelessWidget {
  const NiliApp({super.key});

  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      debugShowCheckedModeBanner: false,
      title: 'NILI',
      theme: ThemeData(
        colorScheme: ColorScheme.fromSeed(
          seedColor: const Color(0xFF3730A3),
        ),
        useMaterial3: true,
      ),
      home: const HomePage(),
    );
  }
}

class HomePage extends StatelessWidget {
  const HomePage({super.key});

  final List<Map<String, String>> categories = const [
    {'name': 'كوفرات', 'icon': '📱'},
    {'name': 'شواحن', 'icon': '🔌'},
    {'name': 'سماعات', 'icon': '🎧'},
    {'name': 'Power Bank', 'icon': '🔋'},
    {'name': 'فيتريات', 'icon': '🛡️'},
  ];

  @override
  Widget build(BuildContext context) {
    return Scaffold(
      appBar: AppBar(
        title: const Text(
          'NILI',
          style: TextStyle(fontWei
