properties([parameters([password(name: 'KEY',description : 'Encryption Key'), string(defaultValue: 'password', name: 'pwd', trim: true)])])
node {  
    stage('Build') {
        
        def records = [['key', 'value'], ['a', 'b']]
        writeCSV file: 'output.csv', records: records, format: CSVFormat.EXCEL
//         def records = [['${params.KEY}', '${params.pwd}']]
//         writeCSV file: 'output.csv', records: records, format: CSVFormat.EXCEL
//         def amap = ["${params.KEY}" : "${params.pwd}"]

//         writeJSON file: 'data.json', json: amap
//         def content = readCSV text: 'key,value\na,b'
//         assert records[0][0] == 'key'
//         assert records[1][1] == 'b'
    }
}
    
