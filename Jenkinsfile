properties([parameters([password(name: 'KEY',description : 'Encryption Key'), string(defaultValue: 'password', name: 'pwd', trim: true)])])
node {  
    stage('Build') {
//         def records = [["${params.KEY}", "${params.pwd}"]]
//         writeCSV file: 'output.csv', records: records, format: CSVFormat.EXCEL
        def amap = ["${params.KEY}" : "${params.pwd}"]

        writeJSON file: 'data.json', json: amap
        echo "this is ${params.KEY}"
    }
}
    
